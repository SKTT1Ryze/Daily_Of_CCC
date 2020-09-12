<!-- +# Daily Of CCC (from 2020/08/07) -->

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



<span id="Day009"></span>

## Day 9 (2020/08/16)
今天完成了 zircon-syscall 和 zircon-loader 层从 zCore 到 zCore-riscv 的迁移。  
准备在 QEMU 中跑起 userboot 的时候，遇到了一个大障碍：  
+ 原版 zCore 需要用到zircon镜像 prebuilt/zircon/x64/userboot.so，这些镜像文件依赖于 Fuchsia 官方镜像，目前 Fuchsia 官方不支持 riscv，因此我目前无法获得适用于 zCore 的 riscv 上的 Fuchsia 镜像。
+ 我的理解是 zCore 现在可以在裸机或 QEMU 上跑 Fuchsia 原生用户程序，而 Fuchsia 官方目前只支持 x86 和 Arm 两种架构，再有由于 Fuchsia 是商业项目，因此他们可能不打算支持 riscv，这样的话想在 zCore 上跑 Fuchsia 用户程序的话道阻且长。  

通过和学长，老师们交流，目前想到以下解决办法：  
+ 写一个简单 Fuchsia 小程序替代 userboot.so，先看看运行效果
+ 利用 loader 层底下的实现暂时先重写一个简陋的 zircon-loader，先让整个框架能跑在 loader 层以上，能在上层环境输出，以达到验证底层代码正确性的效果
+ 参照 rCore-Tutorial，整个重写 zircon-loader，不执着于跑 Fuchsia 用户程序的思路，而是跑自己用 Rust 写的用户程序

明天再深入研究一下 zircon-loader 代码，并思考一下后续工作如何开展。  

今天 LPL 季后赛 LGD 3：0 IG，惊呆我了。本来觉得 LGD 有可能赢，但没想到是连续碾压三局，一场 BO5 下来只用了一个多小时。  
小花生还是猛啊，LGD 这老年三叉戟太顶了，就好像那句话：我虽然老了，但是你大爷还是你大爷。  
puff 还是菜得可以，ning 也被小花生压制，IG 还是中上是大爹，队友都有点拉跨。  
明天再忙一天实习的任务，后天就要开始复习考试了。  

<span id="Day010"></span>

## Day 10 (2020/08/17)
今天做了一些尝试。  
首先是打算写一个盗版的 run_userboot 函数，让它加载一个 elf 文件然后创建一个主线程去执行它。运行起来后不出意料地出现 unimplement! 或者 panic!。  
通过 rCore-Tutorial 中提供的 riscv64-unknown-elf-gdb 调试器调试加上一次打 log 重新编译运行，跟踪到 unimplement! 或者 panic! 出现的地方，试图排除 bug。但到最后发现很多出 panic 的原因是在 unsafe 代码中，这样一来就很难查出错误出在哪，毕竟 zCore 中加载的是 Fuchsia 官方镜像，而我这里只是随便找一个 elf 文件来加载，肯定问题会很多。  
然后我就再写了一个更简单的 simple_run_userboot 函数，在这个函数中只提取出 elf 文件的入口地点，交给 proc.start 去运行。这样一来 panic 就不再出现了，程序应该是跳到了某个地址中执行，但是没有输出。  
目前带来了一个新的问题就是：zCore 是对接 Fuchsia 用户程序的，如果我们不想对接 Fuchsia 而是 Rust 编译的面向 riscv 平台的程序的话，底下的内核实现需不需要改？要改多少？  
另外就是我目前不清楚 zCore 里面的文件系统是怎么实现的，需要花时间去理解一下代码。  
在上述的尝试过程中，途中遇到了一些 unimplement，我对其中的一些进行了实现或者暂时写了一些粗糙的实现，以让我的代码能跑在用户态。具体整理如下：  
+ 用 kernel-hal 中 unimplement 的函数中加上 kernel-hal-bare 中实现的函数链接，让代码转到 kernel-bare 中执行
+ 重写 memory 模块，实现了页帧分配器（使用现成的），al_frame_alloc，hal_frame_alloc_contiguous，hal_frame_dealloc 这三个在 kernel-hal 中定义但没有实现的函数，目前页帧分配已经可以正确使用
+ 将 print! 和 println! 宏从 console.rs 转到了 logging.rs，更好地对接原 zCore 的实现
+ 之前如果代码使用了 kcounter 相关的功能话，会报链接错误，现在修改了 linker.ld 文件使得代码可以正确链接
+ 在 thread.start 函数中原本没有在 riscv 平台下对 context 的处理，我这里为其加上了一些简单的实现，正确与否还得在后续的开发中观察和修改
+ 为某些实现增加了一些共用的成员函数，以便我可以写测试代码

目前的进展大概就到这，往后要复习考试，可能会停滞一些了，在复习期间可能会抽时间给 zCore 加一点单元测试，争取在月底能在力所能及的范围做尽量多的事。  

今晚打了几局 LOL，玩了一把厄菲流斯，在前期大劣势的情况下后面几波团战输出拉满，最终完成翻盘。这英雄连削了九次，削成这样了还能 c 我是没想到的。还打了几盘大乱斗，大乱斗是真的好玩hhh。  
明天开始复习，今天放松一下。  

pass：luojia 的 RIOS组织报告的会议记录：  
> RIOS组织正在达成一个五年目标，提出了一个称作PicoRio的开放架构。希望能减少开发者的开销，有一款文档详细的单板计算机，功率要和树莓派板子对标。 PicoRio的开发分为三个阶段，第一阶段希望实现异构多核的处理器，要实现还在草稿中的RISC-V的动态语言J扩展，跑Linux，跑Chrome OS的内核。希望在今年秋天发布第一个版本。 第二个阶段希望支持图形处理器，希望支持虚拟机监视器，希望有一个WebAssembly的运行时。第三个阶段希望有更多的工业软件和更好的性能。
> J扩展正在草稿阶段，可能要增加两个功能。还在讨论过程中。 增加一些CSR，增加一些地址保护的模块。非常早期。


<span id="Day015"></span>

## Day 15 (2020/08/22)
今天下午参加会议，与老师和学长们说了目前的进展和遇到的障碍，和正在准备考试的情况。经过讨论，向老师同意我放弃对接 Fuchsia 的观点，并且提出一个看起来可行的建议：往 Linux 方向走。  
因为我之前一直都是往 zCore 跑 zircon 程序这条线上走的，这条路走到用 zircon-loader 加载 Fuchsia 镜像时就走不通了，因为 Fuchsia 不支持 riscv。  
向老师说走 Linux 这条路可能能行，因为在 rCore 上已经得到验证了。这样一来我打算在复习的空余时间继续按这个思路尝试一下。  
另外向老师说可能会邀请我们学校操作系统课的老师来听我们的最终项目报告，我觉得这是好事，可以推动国内高校的操作系统课程教育的发展，而不是永远都是老一套。  
今天晚上开始将 zCore 里面的 linux-object 层移到我搭建的运行环境中，但遇到了一些问题，问题来源于 linux-object 层依赖于 zircon-object 层，而 zircon-object 层相比于我一开始移植的时候已经有较大的变化，因此我需要修改一下 zircon-object 层的实现。  
今天的会议很有意义，让放松了几天的我重新回到工作状态上。明天继续加油。  
今天 TES 3：0 SN，成功晋级 LPL 夏季赛总决赛同时获得了 s10 全球总决赛的门票。这是 knight 第一次 s 赛之旅，希望不留遗憾。卡萨连续第 6 次进入 s 赛，出道到现在从未缺席，有点厉害。水手组合冲！  

<span id="Day016"></span>

## Day 16 (2020/08/23)
今天白天复习考试，晚上继续实习任务。  
今天晚上修复了 zCore-riscv 的代码版本落后于新版本 zCore 的问题，具体来讲是新版 zCore 中有关进程的某些实现改了，因此我大致上是将 zircon-object 层重新移植了一遍。  
同时将 zCore 中的 linux-syscall 层移到了运行环境中，只是目前还没有增加测试来验证代码正确性。  
今天 jdg 3-1 lgd 成功晋级 LPL 夏季总决赛同时也获得了 s10 全球总决赛的门票，也将在决赛中重演“春决之战”。老干爹可惜了，不过还有冒泡赛打，而且有两条命，希望小花生能再次进入 s 赛。  

<span id="Day017"></span>

## Day 17 (2020/08/24)
今天同样是白天复习考试，晚上做实习任务。  
之前修改了 zircon-object 的代码，导致测试模块无法编译。今晚修复了这部分 bug，现在测试模块可以正常进行测试了。但是有一个测试就是 job_test.rs 中的 create 测试无法通过，原因不明。去到原 zCore 中的对应的测试模块进行测试，同样该测试无法通过，因此可能是测试本身有问题，因此把出错的那行 assert 去掉后测试可以正常通过。  
修改了 vmo 相关的测试模块，目前可以成功编译，但和之前一样测试无法通过，原因应该是底下的某些实现没有写对，这个要等考完试之后才能慢慢来修改。  
今天开始了两部番的补番计划：《谜之彼女X》和《成群结伴！西顿学院》。都挺好看的，打算利用空余时间来补这两部番。  


<span id="Day018"></span>

## Day 18 (2020/08/25)
今天也是利用了晚上的一点时间来做实习任务。  
先是将 zCore 中的 linux-loader 层移了过来，并且增加了一些测试。同时大致地浏览了一遍 linux-object 层的代码，发现这些代码在建立在 zircon-object 之上的，很多地方都是在定义一个 trait，然后为 zircon-object 里面的结构实现这个 trait。  
现在的问题是我不太清楚在 zCore 中是怎么在 linux 分支里运行起来的，并且发现我缺少了很重要的一个步骤：阅读 Makefile。我需要阅读 zCore 的 Makefile，理解它是怎么在 QEMU 中运行起来的。  
明天将开始阅读 Makefile。  

<span id="Day019"></span>

## Day 19 (2020/08/26)
按照计划，今晚阅读一下 zCore 的 Makefile。  
经过今晚较短时间的阅读，对 zCore 是怎样在 QEMU 中跑起来的有了大概的认识，但还需要更深一步的阅读和理解。   

<span id="Day022"></span>

## Day 22 (2020/08/29)
今天是华科本科生老生回校的日子，我早上 7 点 22 在广州南站出发，中午 12 点多回到了阔别半年的华科。回到寝室已经 1 点左右了，简单收拾一下然后开始准备下午的会议。  
会议中我第二个发言，我主要讲了我这个月在 zCore 到 riscv 上的进展，然后讲了后续工作的开展方向。讲得不是很好，这个是讲稿的地址：[zcore_practice_report](https://github.com/SKTT1Ryze/zCore-riscv/blob/master/zcore_practice_report.pdf)   
luojia 同学是最后一个发言，这里就有话可说了，luojia 将这个发言机会当成了宣传 Rust 的机会，整个会议顿时就换了一个画风，变成了大型 Rust 传教现场。当然 luojia 同学也不是全都是讲 Rust，他还讲了 riscv，OS 的一些内容。他讲得特别好，被某个来参的其他学校的老师称“想像不到这是一个大二的学生在讲”。也有老师说“学到了很多东西。”  
最后被邀请来参加会议的老师们点评，最主要的一点就是，我们在进行汇报的时候，他们不清楚我们做的东西的背景，导致听得不是很懂。  
这个暑期实习到此就差不多结束了，感谢我自己这两个月的付出和各位同学老师的陪伴。  
终于回到了心心念念的大学校园，感到十分开心，在家总是一个人在学习，看动漫，没有人可以一起分享，我得珍惜现在所剩不多的大学生活了。  

<span id="Day023"></span>

## Day 23 (2020/08/30)
今天白天基本上都是在复习。  
晚上和舍友去吃火锅。  
今晚 LPL 冒泡赛 LGD 3：1 IG，顺利挤掉 IG 进入全球总决赛。  
自此 LPL 的四只征战 s10 的战队分别是 TES，JDG，SN，LGD。  
为 LPL 获得 s 赛冠军的 FPX 和 IG 都无缘本次全球总决赛。  
快乐家族 LGD 时隔 5 年再次杀入全球总决赛，真的不容易。自从伟神当年那一箭，LGD 就一直徘徊在季后赛大门之外。如今五个老将，在今年夏天聚在一起，挑战光阴，最终跌跌撞撞闯入了 s10,真的令人感慨。特别是小花生，是我最喜欢的一位大野选手，他和那支传奇战队 ROX Tiger，一起带给了我电竞的激情。希望他能在 s10 上走得更远。  

<span id="Day024"></span>

## Day 24 (2020/08/31)
今天下午考的是汇编，考得挺简单的，做得挺顺利的。  
和一个很熟的学长一起吃晚饭，他已经在电气学院保研了，现在他很闲，经常在宿舍打游戏。应该在我大四的时候还能在华科看到他，只不过他那时候已经是研究生了。  
下一门是数电，今晚不想复习了，要把握这么珍贵的时间去做一些更有意义的事情。  

<span id="Day025"></span>

## Day 25 (2020/09/01)
今天一天复习数电考试，这门考试不是很难，复习起来还算比较轻松。  

<span id="Day026"></span>

## Day 26 (2020/09/02)
今天下午考完了数电，数电中实验的那部分题出得有点坑，其他还好。自启动这个知识点没复习到，不过影响不大。  
晚上写好了 8 月 zCore 实习的书面报告，并和向勇老师聊了一会。他鼓励我继续做我感兴趣的事情，我觉得向勇老师是不可多得的好老师。  
自己还要加把劲，成为更好的自己。  

<span id="Day027"></span>

## Day 27 (2020/09/03)
今天一天复习模电考试，感觉这门课比较难，得好好复习。  

<span id="Day028"></span>

## Day 28 (2020/09/04)
今天下午考完了模电，这次模电考试考了很多课本里面的内容，但这部分课本内容我记不太清楚了，不过这卷子做起来还行，基本上都会做。  
晚上玩了几把英雄联盟，很久没在宿舍玩 LOL 了，不太习惯，玩得有点拉跨。明天复习最后一门信号与系统，再加把劲。  

<span id="Day029"></span>

## Day 29 (2020/09/05)
今天一天复习信号与系统。这门课之前没有好好学，很多东西都要记，比如常用的单边傅里叶变换，拉普拉斯变换，z 变换。还有各种变换的性质。  
今晚是战斗之夜，赶紧打了一把人机就复习去了。  

<span id="Day030"></span>

## Day 30 (2020/09/06)
今天终于考完试了！起飞！早上的信号试卷有点恶心，不过都过去了不想理会了。  
晚上和舍友加上一个同班同学 5 个人一起去呷普呷普吃火锅，这次聚餐体验很好，和同学聊了很多学术上的东西，菜也好吃。  
晚上回寝室写 Rust 代码，将《Rust 程序设计语言》这本书里面的最后一章的小项目：一个小 web server，重新实现了一遍，主要是将它模块化了。  
打算睡觉前补一下《春物》，我上一次看《春物》还是在 7 月份。  
明天是今年的第一次课，经历许久又将再次回到大学课堂了。晚安。  

<span id="Day031"></span>

## Day 31 (2020/09/07)
今天是新学期的第一天上课，阔别整个大二下学期之后重新回到课堂上，甚是感慨。  
第一节课是计算机网络，感觉这门课的老师讲得不是很好，虽说语速适中，但是老是在扯东扯西，很少讲到核心的学术知识。  
上午第二节课是大数据处理，这门课的老师就讲得比较好了，平易近人，懂得也很多，比如说 docker 这个比较新的技术都了解得挺深刻的，看来选这门课选对了。这门课最后是单人项目的考核方式，我也正是比较喜欢这种形式。  
下午第一节课是操作系统原理课。讲师是一个女老师，叫做谢夏。一开始没有对这个老师抱很大的期望，因为我已经见识了清华大学的向勇和陈渝两位老师。不过这节课听下来，顿时对这个老师的好感上升不少。她讲课很活泼，一些理论讲得也很清楚，关键是她懂比较多操作系统方面的知识。还是很不错的。  
晚上为前几天写的 mini-web-server 添加了一个线程池，实现用管道进行线程间通信。在这个过程中补了一下 Rust 的基础知识：  
+ 错误处理
+ 并发编程
+ 闭包
+ 优雅停机处理

最后将代码整理了一下，这个练手项目就到此结束了。  
除此之外我还尝试了使用 Rust + Gtk 进行了图形界面的开发，具体就是用 Glade 绘制 UI 界面和调用 Rust 的 Gtk 相关 crate，最后成功运行起一个 Gtk 窗口。感觉如果有时间的话可以再深入了解一下然后用 Rust + Gtk 写个游戏。  
打算明天开始一边深入学习 Rust 语言一边继续 zCore 到 riscv 移植的工作。  
看邮箱的时候突然发现金海教授回我了，我是中午才发的邮件，希望到他实验室去进行科研学习。这速度有点快啊，有点开心。  
看了《春物》第三季第四集，看到最后真的好心疼团子。大老师也太难了，要在两个里面选一个，明明两个都是 大切な人。真的不希望她们三个中的任何一个人受伤呜呜呜。  
晚安。  　

<span id="Day032"></span>

## Day 32 (2020/09/08)
今天早上上了这学期的第一节计算机组成原理课，发现这门课和操作系统原理，编译原理，接口技术这三门课都有很大的联系。四门课程知识环环相扣，最终学完这四门课之后会有一个系统综合能力实验。感觉很有趣。在 PPT 上看到这个系统综合能力实践有一个课题是写 RISCV 的 OS 微内核，这就是清华大学的王润基学长他们已经做过的 rCore 了，但是 rCore 不是微内核，要是 zCore 能移植到 riscv 上就应该可以了。下课后跟老师聊了一下，谈了一些关于龙芯杯，计算机体系结构，操作系统的一些话题，并了解到我们学校有个老师正在做 RISCV 上的操作系统相关的事情。我打算这段时间联系一下他，并想和他交流一下想法。  
下午继续 zCore 到 riscv 的移植，很高兴有了一些小小的进展：pmem_test 可以通过了，还修了一些其他地方的东西，虽然进展很小，但是也足够令人高兴。  
晚上自己尝试用 Rust 写一个线程池，当作是 Rust 的训练项目。最后虽然那大致完成了，但是还有一些 bug 要修。我希望通过写一些项目来逐渐提升我的代码能力和工程能力。  
今晚 T1 3：1 AF，CUZZ 和 Teddy 终于被换下去了，没有了指挥权的争夺，顿时像换了一个队。你李哥还是你李哥。明天打 GEN，T1 加油！  
晚安。  

<span id="Day033"></span>

## Day 33 (2020/09/09)
今天早上去找金海教授，和他聊了会出国的意愿和想进行 RISCV 和操作系统方向的科研。他把我推荐给了邵志远老师，邵老师正在做 RISCV 相关的研究，而且他也是卓越工程师班的操作系统老师。和邵老师聊了聊，了解到他正打算开启一个科研项目，关于 RISCV 的虚拟化这样的一个东西。另外还他让我加入了计算机卓越班的操作系统课程群，让我先做一下他们的实验：基于 RISCV 的代理内核的操作系统课程实验与课程设计。我稍微看了一下实验指导书的第一章第二章，发现有点意思，打算下午上完计算机网络的课后回寝室做一下这个实验。  
这个实验是基于 riscv 的代理内核（Proxy Kernel) 来进行的，代理内核可以看成是操作系统的一个极小子集。  
为什么选择用代理内核：  
+ 如果采用完整内核的思路来设计实验，非常容易陷入某个模块比如启动，中断处理，内存管理等设计细节。
+ 完整方案中即使是为了运行一个最简单的 HelloWorld 程序，都需要实现如用户态进程封装，进程调度等以及之前的一系列操作系统模块，这样做反而忽略了操作系统对硬件进行封装以支撑应用运行的本质。
+ 同时完整操作系统内核实验方案往往需要自己写一个简单文件系统，并用它来组织虚拟磁盘，这样就不得不引入大量与应用支撑无关的代码，导致了工程庞大和重点不突出等诸多问题。

代理内核的存在是为了在硬件（模拟器）上支撑应用，而设计的最小化的操作系统内核。它可以根据应用的复杂度的不同，调整自身的复杂度。从学习操作系统知识的角度来看，代理内核的这些特点更有利于站在应用的角度来审视操作系统对硬件的封装和为应用所做的支撑，从而更好地理解从原理课程所学到的知识。  


现代处理器定义不同特权级的根本原因，是为了对操作系统进行保护。例如让操作系统运行在较高的特权级，而用户代码则运行在较低的特权级，以防止用户态代码执行恶意的动作破坏操作系统。有时候用户态代码会在它的生命周期里要求做一些“合法“的特权级行为，例如进行 I/O，这就意味着处理器需要支持特权模式的转换，在 riscv 中实现这种转换的工具就是中断。riscv 处理器可以实现跨特权模式的转换，例如从 U 态进入 M 态，或者从 M 态返回 U 态，取决于机器的状态寄存器的设置。  
特权级寄存器：  
+ mscratch：M 态的栈顶指针
+ mstatus：中断处理程序的入口地址
+ mepc：异常指令的地址
+ mcause：中断的原因
+ mtval：异常的参数值，比如缺页异常时访问的虚拟地址
+ mie：中断开启寄存器
+ mip：中断等待寄存器
+ mideleg：中断代理寄存器
+ medeleg：异常代理寄存器

借鉴参考文献[SiFive Interrupt]的中断分类标准，将系统中发生的能够中断当前执行代码的事件分为 3 种：  
+ Exception：条件不满足，例如除零错误，缺页，权限不够。处理完毕后，系统返回发生 exception 的那条指令重新执行
+ Trap：即系统调用或者软件中断，由当前执行的程序主动发出，比如屏幕输出，磁盘文件读写。在 riscv 中，trap 的产生是由特定指令 ecall 导致的。不同于 exception，trap 在处理完成后返回的是下一条指令
+ Interrupt：一般是由外部设备产生的事件而导致的，比如 timer 事件，I/O 完成等。interrupt 在处理完成后返回的是下一条指令。

RV64G 处理器在发生中断后，会将发生的中断类型，编号自动记录到目标模式的 CSR 中。假设发生中断的目标模式是 M 模式，则中断的这些信息会记录到 mcause 寄存器。  
当发生的中断类型是 interrupt 时，mcause 的高位为 1,而如果发生的中断类型是 exception 或 trap，mcause 的高位则为 0。  
对于 M 态，interrupt 的 code 字段的可能取值和含义为：  
+ 3：Machine software interrupt。软件产生的中断但却不是 exception 或 trap。主要是指在多核（Harts）环境下的处理期间中断。riscv 通过让一个核直接写另外一个核的本地中断控制器来实现这类中断。这个不是软件中断或者 trap。
+ 7：Machine timer interrupt。时钟中断。
+ 11：Machine external interrupt。除了时钟中断之外的其他机器中断，例如键盘和其他外设。
+ >=16：Implementation defined local interrupts。与实现相关的其他中断源。  

非 interrupt：  
+ code = 8：来自 U 态的 trap
+ code = 9：来自 S 态的 trap
+ code = 11：来自 M 态的 trap
+ 其余的情况都是 exception，比如 code = 13 的缺页异常

中断向量表的组织和实现方式：  
+ 直接模式
+ 向量模式

riscv 根据 mtvec 的最低位（mtvec.mode）来判断系统具体采用哪种模式。  

当发生一个中断，假设目标模式是 M 模式，riscv 处理器将会这样做：  
+ 保存 pc 到 mepc
+ 将发生中断前的特权级保存到 mstatus 寄存器的 MPP 字段 
+ 设置 mcause
+ 将 pc 设置为中断例程的入口，如果为直接模式则设置为 mtvec 的值
+ 将 mstatus 的 MIE 字段清零，转入机器模式

中断处理例程伪代码一般这样写：  

```riscv-asm
    .align 6
    .global handler_interrupt
handler_interrupt:
    addi sp, sp, -32*REGBYTES
    STORE x1, 1*REGBYTES(sp)
    STORE x2, 2*REGBYTES(sp)
    ...
    STORE x31, 31*REGBYTES(sp)
    call software_handler
    LOAD x1, 1*REGBYTES(sp)
    LOAD x2, 2*REGBYTES(sp)
    ...
    LOAD x31, 31*REGBYTES(sp)
    addi sp, sp, 32*REGBYTES
    mret
```

执行 mret 指令时：  
+ 将 mstatus 的 MPIE 字段恢复到 MIE 字段
+ CPU 转换到 mstatus 中 MPP 字段所对应的特权模式
+ 将 mepc 中的内容恢复到 pc 中

riscv 的中断代理机制：  
riscv 中可以将系统中的特定中断或者异常，通过设置较高特权级的 CSR 寄存器，“代理给”某个更低的特权级处理。比如可以设置 M 态的 mideleg 以及 medeleg 中的某些位，将系统中的部分中断（对应 mideleg）或异常（对应 medeleg）“代理”给 S 态处理。  

页式虚拟存储管理：  
+ 采用 RV64G 指令集的 riscv 处理器在 S 态提供了三种虚拟内存管理方式：Bare，Sv39 和 Sv48。
+ Sv39 虚存管理方式实际上只用到了 64 位中的 39 位。
+ 39 位逻辑地址划分：VPN[2](9),VPN[1](9),VPN[0](9),page_offset(12)
+ 地址变换是由 riscv 处理器硬件完成的，但是页表的构造却是操作系统的重要任务
+ 对于操作系统中运行的每个进程，都应该有个一页表与其对应，当 CPU 需要执行某个进程的时候，就应该将 satp 指向想要执行的进程。
+ 对于一个进程而言，它可能用不满全部虚拟地址空间，这种情况下它的页表中可能只有非常少的部分的 PDE/PTE 是有效的，而其他 PDE/PTE 并不指向任何物理内存页面
+ 若要将操作系统本身的地址空间部分开放给某用户进程，有了页表的帮助，这种共享必须考虑到权限问题，但是必须考虑到权限问题
+ 为了加快虚拟地址到实地址的转换，今天的 CPU （包括 riscv）一般都内置了 TLB 单元，其速度接近寄存器。在进行地址转换时，将常用的 PDE/PTE 存储在 TLB 中以加速虚实地址的转换速度。有个问题是当发生进程切换时，TLB 中很有可能还保留了上一个进程的地址变换所涉及的 PDE/PTE。这时，我们就需要借助 satp 寄存器中的 ASID 字段来判断是否发生了进程切换，如果发生了，操作系统就需要调用 SFENCE.VMA 指令来将 TLB 中的内容刷新。  
+ 对于 2MB 的兆页，只需要将虚拟地址部分的 VPN[0] 和 VPN[1] 都当作页内偏移即可。  

呜呜呜今晚李哥输了，今年世界赛又看不到李相赫了。李哥继续加油吧，上山的凡人没资格嘲笑下山的神。  

<span id="Day034"></span>

## Day 34 (2020/09/10)
今天做了下学姐给我发的实验，目前做完了实验二。  
实验一就是在 proxy kernel 源码中挖几个空让做实验的人去填，比较简单，即使不会做也可以直接看源码。  
但是在做实验二的过程中遇到一个问题：proxy kernel 中 trapframe 的实现，有个叫做 insn 的成员，我看了好一会源码，还查阅了很多 riscv 相关的文档，还是不太清楚这个 insn 是个什么东西。感觉是这个开源项目 proxy kernel 自己的设计。目前还是一脸懵。  
现在我有个感觉很有趣的想法：用 Rust 语言来重写这个 proxy kernel，使得我们可以得到一个用 Rust 语言写的代理内核，我们可以这样运行我们的 riscv 代码：  
```shell
spike rust-pk hello_world
```
想想就觉得很有趣，感觉这是一个很好的 Rust 项目。但是目前不知道可不可行，改天问下洛佳看看他怎么看。  
另外可以看看 spike 和 pk 是怎么结合运作的，并学习一下代理内核的概念。  
晚上和学姐聊了聊，跟她说了几个实验文档里面的错误，并且跟她约好了周日上午去她实验室交流一下关于这个实验的一些问题。  
这个实验还是可以的，我通过这个实验的确熟悉了一些 riscv 的特权级设计。  
今天邵老师发了一个关于 Arm 虚拟化的 PPT，今天还没时间看，明天找时间看一下。  
晚安。  


<span id="Day035"></span>

## Day 35 (2020/09/11)

Virtualization is the process of running a virtual instance of a computer system in a layer abstracted from the actual hardware. Most commonly, it refers to running multiple operating systems on a computer system simultaneously.  
Hypervisor:  
+ bare metal, run guest virtual machines directly on a system's hardware
+ hosted, behave more like traditional applications

KVM, short for kernel-based virtual machine, is a part of the Linux kernel that can run virtual machines directly, although you can still use a system running KVM virtual machines as a normal computer itself.  

A virtual machine is the emulated equivalent of a computer system that runs on top of another system. Virtual machines may have access to any number of resources: computing power, through hardware-assisted but limited access to the host machine's CPU and memory.  

A container is actually just an isolated process that shared the same Linux kernel as the host operating system, as well as the libraries and other files needed for the execution of the program running inside of the container, often with a network interface such that the container can be exposed to the world in the same way as a virtual machine.  

上面是早上看的一些关于虚拟化和 Hypervisor 和 容器的介绍。  

今天下午睡了会觉，醒来差不多四点了，收拾收拾上课去了。  
晚上本来准备赶快做完焦学姐设计的实验三然后看邵老师早上给我发的关于虚拟化的论文，但没想到一做就是一晚上。原因是一开始我没有看实验指导书后面的基础知识，那里有学姐加上的代码解释，方便我们读懂她写的内存管理模块代码。这导致我靠自己分析学姐的代码然后做这个实验，最后花的时间就比较长。不过还是锻炼了代码能力还是有好处的。  
明天早上再早点起来看一下关于虚拟化的论文吧。  
刚刚填了个 Rust 社区调查表，希望 Rust 越来越好，有种你们 20 年后不用 Rust！  
晚安。  