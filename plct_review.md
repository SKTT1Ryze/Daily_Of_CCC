---
marp: true
---
<!-- 中科院软件所 PLCT 实验室实习申请技术报告 -->
<!-- 2021-03-24 -->

# **RISC-V 与 Rust 语言与嵌入式**
华中科技大学计算机科学与技术学院  
车春池  
2021-03-24  
[email](linuxgnulover@gmail.com)  
[github](https://github.com/SKTT1Ryze)  

---

<!-- 注意：报告过程中需要多点技术细节 -->

## **Outline**
+ RISC-V 生态
+ Rust 语言
+ RISC-V 与嵌入式
+ Rust 语言与嵌入式
+ Rust 语言与 RISC-V 嵌入式

---

## **RISC-V 生态**
+ 开放的精简指令集架构，完全开源，设计简洁，模块化设计（基本指令集 + 扩展指令集）
+ 与 X86 架构对比：简化芯片开发，抛弃历史包裹，但目前在高性能处理核领域稍逊
+ 与 Arm 架构对比：开放，大道至简，但生态上需要进一步发展

---

## **RISC-V 生态**
**RISC-V 在嵌入式领域大有可为**  
“对比 Arm, RISC-V 在成本，功耗，性能上目前都没有显著的优势，”，国内某知名芯片厂商产品经理，“但 RISC-V 的开放性会给嵌入式行业带来一个新的模式。”  
（出处：2020-12-26 全国操作系统大赛研讨会现场台下）

---

## **RISC-V 与嵌入式**
+ 功耗与性能：和 Arm 不分上下
+ 成本：对比 Arm 较低
    - 设计成本较低：简洁的设计风格（规整的指令结构，简单的寄存器组成），模块化
    <!-- - 维护成本较低：todo -->
    - 架构授权：完全开源，而 Arm 需要支付昂贵的授权费
+ SBI 标准，便于移植运行在 S 态的操作系统

---

## **Rust 语言**
+ **21 世纪的语言新星**(ref: luojia)
+ Rust 的**安全哲学**
+ 所有权，生命周期
+ 无垃圾回收，极小的运行时，同时兼顾安全与高效

---

## **所有权**
```Rust
// s 是这个字符串值的所有者
let s = String::from("hello_world");
println!("{}", s);
// 将所有权转移到 c 变量
let c = s;
// 尝试打印 s 的值，但 s 的所有权已经转移，因此编译器会报错
println!("{}", s);
```
编译器报错：  
```
error[E0382]: borrow of moved value: `s`
  --> src/main.rs:10:20
   |
3  |     let s = String::from("hello_world");
   |         - move occurs because `s` has type `String`, which does not implement the `Copy` trait
...
7  |     let c = s;
   |             - value moved here
...
10 |     println!("{}", s);
   |                    ^ value borrowed here after move
```

---

## **所有权**
```Rust
// s 是这个字符串值的所有者
let s = String::from("hello_world");
println!("{}", s);
// c 获得 s 的借用
let c = &s;
// s 的所有权没有转移，因此可以成功编译
println!("{}", s);
```

---
## **生命周期机制**
```Rust
// 定义一个引用
let r;
{
    let s = String::from("lifetime");
    // r 获取字符串 s 的引用
    r = &s;
} // s 的值在这里被丢弃
// 尝试使用 r 的值，编译报错
println!("r: {}", r);
```
---

## **生命周期机制**
编译器报错：  
```
error[E0597]: `s` does not live long enough
  --> src/main.rs:8:13
   |
8  |         r = &s;
   |             ^^ borrowed value does not live long enough
9  |     } // s 的值在这里被丢弃
   |     - `s` dropped here while still borrowed
...
12 |     println!("r: {}", r);
   |                       - borrow later used here
```

---
## **生命周期注解**
ref: https://kaisery.github.io/trpl-zh-cn/ch10-03-lifetime-syntax.html  
```Rust
fn longest(x: &str, y: &str) -> &str {
    if x.len() > y.len() {
        x
    } else {
        y
    }
}
```
编译器报错：  
```
error[E0106]: missing lifetime specifier
 --> src/main.rs:5:33
  |
5 | fn longest(x: &str, y: &str) -> &str {
  |               ----     ----     ^ expected named lifetime parameter
  |
  = help: this function's return type contains a borrowed value, but the signature does not say whether it is borrowed from `x` or `y`
help: consider introducing a named lifetime parameter
  |
5 | fn longest<'a>(x: &'a str, y: &'a str) -> &'a str {
  |           ^^^^    ^^^^^^^     ^^^^^^^     ^^^
```

---
## **生命周期注解**
ref: https://kaisery.github.io/trpl-zh-cn/ch10-03-lifetime-syntax.html  
```Rust
fn longest<'a>(x: &'a str, y: &'a str) -> &'a str {
    if x.len() > y.len() {
        x
    } else {
        y
    }
}
```

---

## **Rust 语言**
+ 强大的类型系统，Trait 语法，支持泛型（常量泛型），函数式编程
+ 友好的包管理（相比 C/C++ 是一个大优势）
+ 卫生宏，过程宏（内部展开，不影响上下文）
+ 成长的社区

---

## **Rust 语言与嵌入式**
**Rust 语言非常适合嵌入式软件开发**  

+ 极小并且可定制的运行时 -> 性能
+ 独特的内存管理 -> 安全（所有权模型 -> 外设抽象）
+ （包管理工具， 强大的宏） -> 生产效率
+ 丰富的编译目标（RISC-V, Arm, MIPS)
+ **异步支持**（最小的异步抽象库 `nb` 和内置的 async/await 语法）

---

## **Rust Async in Embedded**
```Rust
use embedded_hal::serial;
impl serial::Read<u8> for UartLite {
    type Error = Infallible;
    fn try_read(&mut self) -> nb::Result<u8, Self::Error> {
        match self.stat_reg.is_set(Status::RX_VALID) {
            true => Ok(self.rx_fifo.get() as u8),
            false => Err(nb::Error::WouldBlock),
        }
    }
}
```

---

## **Rust 语言与嵌入式**
**Rust 嵌入式生态**   
![rust_emebdded](./rust_embedded.png)  
[ref](https://github.com/rustcc/RustChinaConf2020/blob/master/rustchinaconf2020/RustChinaConf2020-17.%E6%B4%9B%E4%BD%B3-%E3%80%8ARust%E8%AF%AD%E8%A8%80%E4%B8%8E%E5%B5%8C%E5%85%A5%E5%BC%8F%E5%BC%80%E5%8F%91%E3%80%8B.pdf)  


---

## **微架构运行时库**
+ 运行第一条**逻辑代码**之前的准备工作
+ 通过过程宏提供函数入口
+ 处理机器模式中断和异常

---

## **embedded-hal 标准**
+ Rust 嵌入式社区统一的标准
+ 这个库是对外设本身的抽象，提供一系列的 Trait,不涉及具体的实现
+ 实现由各个开发版（SoC）的实现库来完成（stm32f30x-hal， k210-hal）
+ 基于特定硬件的外设访问库来实现

---

## **Rust Async in Embedded**
```Rust
use embedded_hal::serial;
impl serial::Read<u8> for UartLite {
    type Error = Infallible;
    fn try_read(&mut self) -> nb::Result<u8, Self::Error> {
        match self.stat_reg.is_set(Status::RX_VALID) {
            true => Ok(self.rx_fifo.get() as u8),
            false => Err(nb::Error::WouldBlock),
        }
    }
}
```

---

## **Rust 语言与 RISC-V 嵌入式**
**以 RustSBI 为样本，对比竞品 OpenSBI 来分析**
+ RISC-V SBI 标准
+ [RustSBI](https://github.com/luojia65/rustsbi)  
+ 2000 多行代码量，对于 k210 平台的支持依赖于 k210-hal 和 k210-pac 这两个嵌入式支持库，得益于 Rust 嵌入式生态
+ 对于 k210 的实现缺陷，通过 RustSBI 来弥补，得益于 SBI 标准的设计优越性
+ RustSBI 模块化设计，对于某个特定的平台（硬件或模拟器），只要提供相应的 pac 库和 hal 库，即可很容易适配

---

## **RustSBI**
```Rust
Trap::Exception(Exception::IllegalInstruction) => {
    let vaddr = mepc::read();
    let ins = unsafe { get_vaddr_u32(vaddr) };
    if ins & 0xFFFFF07F == 0xC0102073 { // rdtime instruction
       todo!()
    } else if ins & 0xFE007FFF == 0x12000073 { // sfence.vma instruction
        // k210 平台上不存在 sfence.vma 指令，但存在 sfence.vm 指令，因此我们在 SBI 里面模拟 sfence.vma 指令执行过程
        // 取出 satp 寄存器的值
        let satp_bits = satp::read().bits();
        // 获取根页表的 ppn
        let ppn = satp_bits & 0xFFF_FFFF_FFFF; // 43..0 PPN WARL
        // 写到 sptbr
        let sptbr_bits = ppn & 0x3F_FFFF_FFFF;
        unsafe { llvm_asm!("csrw 0x180, $0"::"r"(sptbr_bits)) }; // write to sptbr
        // enable paging (in v1.9.1, mstatus: | 28..24 VM[4:0] WARL | ... )
        let mut mstatus_bits: usize; 
        unsafe { llvm_asm!("csrr $0, mstatus":"=r"(mstatus_bits)) };
        mstatus_bits &= !0x1F00_0000;
        mstatus_bits |= 9 << 24; 
        unsafe { llvm_asm!("csrw mstatus, $0"::"r"(mstatus_bits)) };
        // 模拟 sfence.vma 指令
        unsafe { llvm_asm!(".word 0x10400073") }; // sfence.vm x0
        mepc::write(mepc::read().wrapping_add(4)); // skip current instruction
    } else {
        panic!("invalid instruction! mepc: {:016x?}, instruction: {:08x?}", mepc::read(), ins);
    }
}
```
---

## **谢谢各位**