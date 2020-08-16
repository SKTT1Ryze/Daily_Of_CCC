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

<span id="Day002"></span>

## Day 2 (2020/08/09)
今天看了一下 zCore 的源码，结合之前看的 pql 学长的毕设论文，目前大概清楚了 zCore 的整体结构。  
经过分析，zCore 中与架构相关的模块在 kernel-hal-bare 文件夹中，我要做的工作就是完善这部分模块对于 RISCV 架构的支持。但目前我对于具体怎么做还没有更明确的认识。  
同时，我还需要对 rCore 中的对 RSICV 支持的代码进行分析，目前在 rCore 源码中有一个 Arch 文件夹，里面是架构相关的代码，我需要重点对这部分代码进行分析。  

<span id="Day003"></span>

## Day 3 (2020/08/10)
今天下了一天 zCore 项目，总是失败，最终还是没有下载完成。  
和罗凯莹去新华书店买书，结果没有买到，然后去了七十二佳房客拍摄地点，但是那里没有开门，然后去菜市场买了菜回家煮饭。  
晚饭罗凯莹提出她来做饭，我打下手。最后做出来的晚饭尝起来还不错。  
晚上就在家里休息。  

<span id="Day004"></span>

## Day 4 (2020/08/11)

今天陪罗凯莹去医院，坐了大概一个小时的公交到那个很偏僻的医院，由于医院设备故障导致需要另行预约。  
我们抛去不愉快的心情去了周围的商场购物，但在结帐的时候我大嫂给的100块钱的购物券用不了，然后我就先付了。  
然后和罗凯莹去了广州购书中心一趟，因为她要买一本叫做《乡土中国》的书。书买好后，我们就回家了。  
晚上思考了一下移植 zCore 的工作要怎么开展。目前打算在 qemu 中跑起 zCore 的 hal 抽象层和内核对象，然后再一步步往上构建。  
今天还算比较不错的一天。  

<span id="Day005"></span>

## Day 5 (2020/08/12)
今天在实习任务上有了一点进展，首先我先尝试把 luojia 维护的 riscv-sbi-rt 库用起来，经过一番尝试并和 luojia 本人的交流后觉得这个库的实现有些问题，因此暂时不用这个库。我使用之前 rCore-Tutorial 的框架搭建了一个 zCore-riscv 的开发环境，目前已经在上面跑起了内核对象。  
下午和罗凯莹去看了《大鱼海棠》，第二次看这部国产电影，还是觉得很震撼，我觉得这是目前国产动画电影的天花板了，特别是作画和特效，是其他国产动画电影无法比拟的。  
晚上是我大嫂煮饭，是我爱吃的混沌。  
买了明天晚上回家的票，得赶快回家工作了。  

<span id="Day006"></span>

## Day 6 (2020/08/13)
今天下午带罗凯莹去美术馆玩。  
看起来她比较喜欢画画，看那些艺术品看得很入迷，我倒是一点也看不懂。  
她马上就要进入高中了，即将迎来很艰苦的三年，祝她好运吧。下次见面可能她已经上大学了。  
晚上我们一起坐地铁，我去广州南站，她转广佛线，我先下车转 2 号线。下车之前向她道了别，下车之后感到些许唏嘘。  
做高铁回到茂名已经 9 点 40 了，叫了辆滴滴回家，一路上看着窗外的夜景一边想着离开家这几天的事情，很是感慨。这将会是我人生中重要的一笔。  
回家快乐。  

<span id="Day007"></span>

## Day 7 (2020/08/14)
今天一整天都在研究 zCore 源码和在我的框架上构建代码，目前对 zCore 源码的分析更新如下：  
+ kernel-hal-bare 模块是唯一与硬件相关的代码
+ zCore 的模块化十分清晰，它将各个层次模块作为一个个 crate 进行调用。比如 kernel-hal 和 kernel-hal-bare。
+ kernel-hal 模块不依赖于其他模块，并为其他模块提供支持
+ 各个模块最终作为一个 crate 在 zCore 中被调用来构建一个 OS
+ 在硬件抽象层之下的 kernel-hal-bare 和 之上的各个层次都有架构相关的代码
+ kernel-hal 模块被其他多个模块依赖，而 kernel-hal-bare 只在最终构建 zCore 的时候被调用
+ 在我构建的框架中，原本在 zCore 中的模块在这里将不再作为一个个 crate，而是一个个 mod
+ 目前的大致方向是在我搭建的这个框架上一点点地构建 os，最终目标是使其能在 riscv 下的 qemu 上执行 zCore 的大部分功能。 


目前我在维护的项目地址：[zCore-riscv](https://github.com/SKTT1Ryze/zCore-riscv)  
在这个项目中我选择将原先在 zCore 中作为 crate 的模块作为 mod 处理的原因有：  
+ 按照之前 rCore-Tutorial 的框架进行开发，会比较熟悉，省去了不少学习的时间成本
+ 这样相当于重新搭建起 zCore，在此过程中我将能较快较全面地熟悉 zCore，理解 zCore 自上而下构建操作系统的思路
+ 如果代码在此框架上能跑通，那么在原 zCore 上也肯定没问题，代码迁移的工作量是很小的


目前进度在 github 上可以看到，目前还比较少。  
争取明天能跑起一个内核对象。  
今天 LPL 季后赛 LGD 打 WE，LGD 3：1WE 挺进 6 强。xiye 和小花生是真的猛，恭喜老干爹时隔 1800 多天再次在季后赛获胜，这只老将组成的队伍一眼看去满满的都是青春啊，老玩家泪目。  
看了一集番：《宇崎ちゃんは遊びたい》，这么可爱的学妹请务必给我来一打！（想屁吃）  

<span id="Day008"></span>

## Day 8 (2020/08/15)
今天完成了 zircon-kernel 从 zCore 到 zCore-riscv 的迁移。  
另外添加了对这部分模块的测试代码，大部分测试都能通过，某些测试因为缺少实现而出现 unimplement panic。  
下面是对 kernel-hal 中 #[linkage = "weak"] 标志的函数的理解：  
+ 这些函数在 kernel-hal 中并没有得到实现，而是由 kernel-hal 层往上的模块实现，这种逻辑的支持来自弱链接
+ kernel-hal-bare 则会是调用后面实现的这些函数，比如 hal_frame_alloc()
+ 在 zCore 中不同模块是分别作为一个个 crate，但是在 zCore-riscv 中是作为一个个 mod，这导致在 zCore-riscv 中不能使用弱链接的形式

解决办法：  
+ 方法一：在各个模块的逻辑中将那些使用 kernel-hal 模块的部分直接换为真正的实现部分
+ 方法二：在后续将 kernel-hal 那些没实现的函数实现之后，在 kernel-hal 里的那些函数体里面调用实现的函数
+ 方法三：重新整理代码将各个模块重构成一个个 crate

使用哪种方法将取决于后面的进展。  
不过无论使用哪种方法，最终都还是要回到 zCore 上去，目前我只是需要在一个运行环境中能成功运行和测试。等在 zCore-riscv 上的运行和测试通过后，各种实现逻辑将会再移植到 zCore 里面去。  
在今天下午的交流会议中，刘丰源学长曾经做过到 mips 上的移植，他给我传授了一些经验：先在一个运行环境中在用户态打印出 HelloWorld，然后再一步步完善底层结果，大致上就是将那些 unimplement 的部分给实现来。  
打算到 18 号开始复习期末考试，这几天尽量做多一点。  

今天 LPL 季后赛 SN 3：1 V5, Sofm 是真的猛啊。  
和昨天一样看了一集番：《宇崎ちゃんは遊びたい》。   
还在 qq 上和罗凯莹聊了一会，她也快开学了，25 号军训。  


















