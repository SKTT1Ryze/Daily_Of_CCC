# Daily Of CCC (from 2020/08/07)

今年暑假我参加了一个很有趣的活动，在这个活动里老师要求我们每天写日志，来记录每天做的事情。我觉得这是一个很有想法而且很有意义的做法，因此在今天晚上，活动的线下实习的最后一晚，我开了另外一个 repo ，在这里每天记录一些东西，比如学习中获得的东西，比如遇到有趣的事情，再比如心情。这个日志独立于我参加实习建立的日志，我希望在这个日志上一直写下去。  

## TOC Day 0~60

* [Day 0](#0)  
* [Day   1](#Day001)   
* [Day   2](#Day002)   
* [Day   3](#Day003)  
* [Day   4](#Day004)  
* [Day   5](#Day005)  
* [Day   6](#Day006)  
* [Day   7](#Day007)  
* [Day   8](#Day008)  
* [Day   9](#Day009)  
* [Day  10](#Day010)  
* [Day  11](#Day011)  
* [Day  12](#Day012)  
* [Day  13](#Day013)  
* [Day  14](#Day014)   
* [Day  15](#Day015)  
* [Day  16](#Day016)  
* [Day  17](#Day017)  
* [Day  18](#Day018)  
* [Day  19](#Day019)  
* [Day  20](#Day020)  
* [Day  21](#Day021)  
* [Day  22](#Day022)  
* [Day  23](#Day023)  
* [Day  24](#Day024)  
* [Day  25](#Day025)
* [Day  26](#Day026)
* [Day  27](#Day027)  
* [Day  28](#Day028)  
* [Day  29](#Day029)  
* [Day  30](#Day030)  
* [Day  31](#Day031) 
* [Day  32](#Day032) 
* [Day  33](#Day033) 
* [Day  34](#Day034) 
* [Day  35](#Day035) 
* [Day  36](#Day036) 
* [Day  37](#Day037)  
* [Day  38](#Day038)  
* [Day  39](#Day039)  
* [Day  40](#Day040)⭐  
* [Day  41](#Day041)  
* [Day  42](#Day042)  
* [Day  43](#Day043)  
* [Day  44](#Day044)  
* [Day  45](#Day045)  
* [Day  46](#Day046)  
* [Day  47](#Day047)  
* [Day  48](#Day048)  
* [Day  49](#Day049)  
* [Day  50](#Day050)  
* [Day  51](#Day051)  
* [Day  52](#Day052)  
* [Day  53](#Day053)  
* [Day  54](#Day054)
* [Day  55](#Day055)
* [Day  56](#Day056)
* [Day  57](#Day057)
* [Day  58](#Day058)⭐
* [Day  59](#Day059)
* [Day  60](#Day060)

<span id="0"></span>

## Day 0 (2020/08/07)
今年 7 月开始到现在我参加了一个实习：  
欢迎在校学生在2020年暑假参加鹏城实验室与清华大学举办的OS Tutorial Summer of Code 2020 活动（7月4日～8月31日），本次活动分为两个阶段rCore Labs Tutorial（7月4日～7月31日）和zCore操作系统实践与研究（8月1日～8月31日） ,主要是对用Rust语言进行OS研发开展学习、交流与探索。  
如有兴趣参加，请发个人简历给 yuchen@tsinghua.edu.cn 并填写调查问卷，获得邀请后，将开始参与如下面所示的rCore Labs Tutorial活动。完成本次活动第一阶段（7月4日～7月31日）的同学如果通过review，将获得鹏城实验室资助到鹏城实验室进行为期一个月的第二阶段（8月1日～8月31日）的OS实习，开展zCore操作系统实践与研究。  
目标：
探索把现代系统语言Rust和灵活开放的系统结构RISC-V带入到操作系统的架构与设计的创新中来，思考未来的操作系统应该是什么样。  
宗旨：
希望本活动的组织，能为操作系统爱好者提供一个活跃的开源社区环境，为对Rust、RISC-V和操作系统感兴趣的人士营造一个平等的学习与交流空间，吸引更多对操作系统感兴趣的人士参与。  
我在上个月通过了 review，在 8 月 2 号来到深圳鹏城实验室进行线下实习，今晚是线下实习的最后一个晚上。  
有那么一群人，尝试使用现代系统语言Rust编写操作系统，探索一个好的操作系统该怎么写，思考未来的操作系统应该是什么样子的。  
这群人的领头羊，就是清华大学教OS课的两个老师和wrj学长，在这些人的带领下，在清华开启了一段用Rust写OS的奇妙之旅。  
他们还尝试将新的架构RISCV结合到编写操作系统上来，并希望他们写的操作系统能在RISCV的真机上跑。  
现在这个想法已经得到了很好的实现，wrj学长起头的rCore操作系统，一个用Rust语言编写的OS已经颇具规模，成长为一个比较健壮，功能较为强大的操作系统。  
而zCore是他们的另一个尝试，这是一个微内核，山寨了Google开发的Zircon微内核，并使用Rust语言编写，充分利用了Rust语言的语法特性，尽管还有许多bug，目前已经能运行在x86架构下了。  
rCore项目已经建立起了一个开发者社区，吸引着许多OS爱好者参与到rCore的开发中来。  
参加这个实习，我很荣幸地加入到这个圈子中来，积极地探索操作系统的奥妙。  
在一周的线下实习过程中，鹏城实验室给我们安排的活动十分丰富，其中最让我感触深刻的是，国科大“一生一芯”团队的5位同学和余子濠博士给我们带来他们完成RISCV处理器的开发过程背后的故事，和去清华伯克利深圳研究所参观，并听了谭章熹博士的关于RISCV的报告(太过前沿，不是很能听懂)。特别是去清华伯克利深圳研究院参观的时候，就像是拜访圣地一样，太激动了  
每天晚上则是wrj等清华研究生学长的关于rCore/zCore的讲座(太强了）  
除此之外，我们还和向勇老师，wrj学长他们进行了一次聚餐，和他们聊天，像做梦一样  
还认识了Rust的疯狂粉丝兼校友luojia同学，太强了  
我参加这次实习受益匪浅，一是Rust语言，二是OS，三是见识。希望我在实习结束的时候能拿出成果来。  
也许许多年后，清华 OS 课的实验就是我们这群人写的hhh。  

<span id="Day001"></span>

## Day 1 (2020/08/08)
今天从深圳做高铁回到广州大哥的家住几天。  
晚上根据 zCore-Tutorial 重现了内核对象的代码，加深了对内核对象的理解。  
下面定义内核对象的 trait ：  
```Rust
/// trait for kernel object
pub trait KernelObject: DowncastSync + Debug {
    /// get id of kernel object
    fn id(&self) -> KoID;
    /// get type of kernel object
    fn type_name(&self) -> &str;
    /// get name of kernel object
    fn name(&self) -> String;
    /// set name of kernel object
    fn set_name(&self, name: &str);
}
```
下面编写一个宏自动为内核对象实现`KernelObject` trait：  
```Rust
#[macro_export]
macro_rules! impl_kobject {
    ($class:ident $( $fn:tt )*) => {
        // implement `KernelObject` trait for object
        impl KernelObject for $class {
            fn id(&self) -> KoID {
                self.base.id
            }
            fn type_name(&self) -> &str {
                stringify!($class)
            }
            fn name(&self) -> alloc::string::String {
                self.base.name()
            }
            fn set_name(&self, name: &str) {
                self.base.set_name(name)
            }
            $( $fn )*
        }
        impl core::fmt::Debug for $class {
            fn fmt(
                &self,
                f: &mut core::fmt::Formatter<'_>,
            ) -> core::result::Result<(),core::fmt::Error> {
                f.debug_tuple(&stringify!($class))
                    .field(&self.id())
                    .field(&self.name())
                    .finish()
            }
        }
    };
}
```
我们还实现了接口到具体类型的向下转换，并为上述逻辑写了单元测试。  