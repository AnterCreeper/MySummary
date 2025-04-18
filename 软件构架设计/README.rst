.. Kenneth Lee 版权所有 2009-2021

:Authors: Kenneth Lee
:Version: 1.0


软件架构设计
************

本文最初作为知乎专栏的README，当时的构思是这样的：::

        前几天发现知乎可以写专栏了，抱着试试看看的心思申请了一下。现在专栏开通了，我的
        感想是：又多一个累赘……

        所以我就构思一下我可以在这里写什么。作为方向性的构思，我先想到如下几条：

        1. 必须写我非常熟悉的，这样我可以少动点脑筋，随口就来。

        2. 因为我是做这一行的，有的是人想探我的底线。所以，这里肯定不会碰我工作有关的方
           向。读者也请不要和我讨论和架构选择相关的问题。这好比打牌，我可以告诉你牌是怎
           么打的，但你不要跑过来看我的底牌

        3. 目标读者。我考虑的目标读者是软件相关领域的从业人员和在校学生。特别是后者。笔
           者读书时的理想一直是当老师，这也算是过个干瘾。另外，自己写软件写了二十多年了
           ，从对软件一无所知到现在也叫有几个成功产品经验了，深感我们国家软件教育之落后
           。这句话不是说要崇洋媚外。笔者职业生涯中，团队中一直不乏来自不同国家的工程师
           ，我们的软件学生确实在基础训练上不如别人。笔者这样说，不是说自己就可以改变什
           么，而是说明，这个Gap是存在的，既然如此，这个事情就可以做。至于做的意义——意
           义这种东西，那是哲学家的问题，我不讨论。

        然后就是写作思路，我的想法是先定软件构架的概念——不是学术的那种概念，而是和读者
        对齐软件构架是什么这个问题。是为了理解上的对齐，而不是严谨的范围区分，这两者的
        区别是什么，读者很快可以看到。然后我会先介绍开发的一些基本的技能，比如怎么做单
        元测试，怎么做数据结构定义等。这些知识看来简单，实际上很多开发者都学错了，在这
        种问题上有错误的理解，后面我们谈什么都没有用，之后我们才会看是谈构架设计上的各
        种考量。

        基本上我会想到哪里写到哪里，根据读者的讨论也会走到不同的方向，欢迎读者一起讨论
        。

        最后，笔者是过来讨论问题的，读者来讨论，无论表达什么观点我都非常感激，但不要指
        望仅过来装逼：）。装逼是一件快乐的事，但失去了要做的事情本身，仅剩下装，这个装
        起来实在很丑。所以，我们要虚心实腹地“顺便装”，不要为装而装，那是很丑的。

        对于软件工程师来说，什么意见会造成Patch的生成，什么意见完全是无效代码，这个其实
        是很清楚的。对于无效代码，如果是无关紧要的tag我不管，但对那些我看不顺眼，解释又
        会浪费逻辑空间的，我不会跟你废话，我会直接删除，所以，Please，装逼可以，请用干
        货装。也许你会说，“难道你就可以肯定你是对的吗？难道你不应该谦虚一点吗？ ”，你说
        得对，我在这个问题上，我就是武断的。这正是软件和自然语言的讨论不同的地方。软件
        每个表述，某种程度上，都是单一结果的，每行代码改进去，我们都预期唯一的结果（唯
        一的含义可以斟酌，但方向是这个方向）。软件工程师是最在乎“断”的人之一了。对的判
        断，和错的判断，对软件工程师来说都是“有效的”，无用的判断，才是无效的。因为软件
        的成本都来自逻辑量（代码量），if(a&b&c&(d|e|f))这个判断如果写反了，前面加一个！
        就解决问题了，但如果这个判断整个写乱了，这个代码就彻底没有用了。


        我说的这个“有效（对/错）/无效”的名称空间就好像老子写《道德经》前面的道可道非常
        道，名可名非常名一样，是全文的根本。后面读者们应该可以看到，我的所有表述，其实
        都是对这个空间定义的证明。

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   什么是软件架构
   大型软件架构设计
   架构师具体设计什么
   Use Case图有什么用？
   使用软件的四种方法
   从单元测试理解软件
   名可名
   小国寡民
   需求分析的中心思路
   关于自然语言编程的方向问题
   反者道之动——欣赏架构设计的基本逻辑
   让代码变立体
   生成优秀的架构
   分支设计要领
   怎样做项目管理
   谈谈子女教育问题
   两种基本的构架表述方法
   弱者道之用——谈技术工作中的守弱问题
   在Linux下做性能分析
   架构设计的0层逻辑
   解耦设计
   怎么做高层设计
   理解架构版本
   PCIE总线的保序模型
   做与不做都是战略
   海洋战术式的软件设计方法
   解耦和不解耦
   再谈“守弱”
   互斥算法设计
   英文版本的“弱者道之用”
   什么是“守”
   从用户功能开始构架系统框架
   Linux发行版的库软件包组织
   地址空间的故事
   工作和读书有什么不同
   怎样快速调试Linux内核
   架构设计中的“少了”和“多了”的问题
   怎样做代码Review
   怎样做客户访谈
   RancherOS架构分析
   再谈什么是软件架构
   大道曰守，当时曰行
   不为天下先
   关于AI的胡说八道
   学习本质？
   “设计的流程”和“代码的流程”
   概要设计不是代码
   “病病”
   关于架构师的爱恨情仇——《黑客帝国》世界观解读
   Linux Socket 0拷贝特性
   用户态DMA的问题
   Multiprocess Support for Linux IOMMU driver
   Linux RAS特性分析
   写论文
   基于“语义”编程
   从学习assert的用法开始理解如何写“专业的程序”
   架构的存在性
   Makefile概念入门
   ARM服务器进展小结
   怎么做初步的需求分析
   关于设计方案中的逻辑链问题
   从逻辑链问题讨论怎么做高层设计
   工程逻辑链
   为什么你会在你的数据中心中部署ARM服务器
   如何为libvirt设置虚拟主机
   给普通人解释Spectre和Meltdown安全漏洞
   给程序员解释Spectre和Meltdown漏洞
   Is retpoline really safe
   逻辑链，道，学和架构工作的本质
   Serverless是什么——谈如何捕获一个特性的架构本质
   道法自然
   自然，守弱和Plan B
   守弱的内涵和外延
   找到道法自然的“度”
   Specification的写法问题
   小姐和丫鬟的故事
   知不知
   PCIE总线的地址问题
   气和深度学习
   单元测试的效果问题
   Requirement Analyzing vs. Voting
   抽离设计逻辑
   盗夸
   抽象还是不抽象的问题
   Tegra TX2一瞥
   Progress and confusion of the IOMMU name space
   一样还是不一样
   运营还是交付
   科普一下GPL和开源软件
   怎么确定道
   回调还是直调
   接口的封装层次问题
   git的基本架构欣赏
   让设计自生
   架构控制的从权问题
   设计的需求问题
   性能优化的目标问题
   加速器和其他硬件的区别
   君子与其练达不若朴鲁与其曲谨不若疏狂
   有无之道——一个新的软件架构定义
   什么是管理
   从香农熵谈设计文档写作
   YVR18资料关注点
   理解关联
   如何撰写技术交底书
   再谈什么是高层设计
   再谈“法自然”的设计思路
   设计规范
   开源交付
   道纪
   X86上的ARM Linux调试环境
   IOMMU的现状和发展
   单元测试的强与弱问题
   做事，做名，绩效主义，以及架构战略
   没有规则的规则
   大成若缺
   非易失内存随想
   参考平台
   一个例子：名的边界效应
   抽象问题的模型
   另一个例子：名的边界效应
   Zircon架构简单分析1：Overview
   在qemu中模拟设备
   国产操作系统问题
   软件飞线
   状态机方法
   一些典型的架构设计错误
   从CPU和TPU的不同语言抽象看抽象原则
   限制管理
   WarpDrive as a General Heterogeneous Platform
   Multiarch概念调查
   ARM NUC
   UML有没有用
   推演一个Buffer分配的语法设计
   架构师和项目经理的基本职责问题
   锁使用设计
   从内核终止用户态程序的IO访问
   epoll和select
   状态机退出方法
   不为天下先2
   设计逻辑和代码逻辑
   流水线深度
   谁是主线？
   理解指令集
   给使用设备的进程发信号
   Linux设备异常复位逻辑分析
   投资开源社区的基本逻辑
   一个Linux死锁信息分析
   如何说谎
   代码生成器
   弟子规：美国军方禁止在C语言程序中使用malloc
   自下而上和自上而下的设计
   正面竞争
   不知为美
   高层封装的设计战略
   产业生态的原理和作用
   弯道问题
   无名概念的深入探讨
   解释On-Chip Debug和Off-Chip Debug
   接口和名称空间辨识
   RISCV WMO和TSO具体解决什么问题
   利益链
   从C的for和Python的for聊起
   安全建模问题讨论
   Accelerator vs. Co-processor
   一个逻辑空间控制的例子：uacce生命周期管理
   软件构架设计的入题角度问题
   接口分层的问题
   对Cache Coherence的重理解
   接口定义的工作模型
   Linux_net和net-next分支的维护策略
   WarpDrive用户态方案重构建议
   主线逻辑
   架构设计的粗与细问题
   狂人日记读后感——名称空间囚笼
   写程序和写小说的区别
   再谈《弟子规》问题
   理解弱内存顺序模型
   思维上的洞2
   后软件时代和技术沙盘陷阱
   怎么做项目管理2
   语言的控制力问题
   分享我的Linux内核开发环境
   开发视图
   概念视图
   处理视图
   语言控制力问题
   新手设计文档典型错误
   讨论：OpenCL2.0SVM有什么好？
   设计逻辑的细致和严密问题
   逻辑的平面和立体问题
   自由和约束
   给非专业人士介绍架构设计工作
   AML工作原理快速调研
   qemu_PCIe总线结构
   ARM64_Linux_Kernel_5.7无法GDB调试问题
   分层抽象
   见素抱朴：一个关于交付的例子
   三个锦囊
   多核MMU和ASID管理逻辑
   PMA和PA方案对比
   真假架构设计
   怎样写标准提案
   安全问题的本质
   名称内涵的发展
   标准和设计的区别
   cond_mutex模型
   一个例子：架构的重要性和从权
   nvdimm_AD模式的内核应用模型
   早期架构设计问题
   所谓内部设计
   “知不知”如何影响决策的？
   “优秀架构设计”
   Linux_Kernel架构赏析
   说说对协程的看法
   架构设计和实施的对齐和同步问题
   一个关于4+1视图的案例：从概念视图开始
   “硬件状态机”
   设计的减熵原理
   架构设计入门知识
   架构设计的大忌：我没错
   “解决方案”
   讨论一下eBPF
   交付中的Version和Revision
   约束选择
   在概念空间选择方案
   git-submodule的理解
   思维的串行化要求
   什么是函数式编程
   管理上的判断和技术上的判断
   基于逻辑链建立约束
   高级需求分析
   False_Sharing
   芯片验证软件的4+1方法
   软件之硬
   诚其意
   把什么放入架构设计
   ARMv8的安全特性的主线逻辑
   指令寻址模式
   线程的本质
   限制的可移动性
   2020年又写的一个什么是架构设计的定义
   正善治
   概念空间建模的要领
   例子和全集定义
   编译阶段和运行阶段算力
   逻辑闭包
   主语问题
   关于概念空间，接口的一些具体讨论
   构架和没错问题的进一步讨论
   专家意见和编辑意见
   架构设计和普通设计的区别
   构架设计的接地气问题
   一个例子——逐句翻译是怎么掐断逻辑链的
   一个逻辑链断裂引起架构设计方向错误的实例
   确定逻辑的根
   机器腔和人类腔
   ABI
   视图和决策面
   架构首先是一种信念
   一个架构设计实例：qemu iommu
   架构的改革属性
   逻辑如水
   综合
   几个架构定义问题的实例
   细节的丢失
   一个架构评审案例
   建模
   逻辑正交
   一些架构引导的例子
   iommu设备和uacce关系分析
   什么叫做没有设计成份
   逻辑闭包的范围管理
   AIA方案的核心优势
   范围问题
   我们是怎么放弃架构的
   uacce_fork问题建模
   设计和科普
   向前兼容数据格式设计
   架构和装修
   关于敏捷项目的一些逻辑
   硬件同步时间差问题的设计逻辑
   抽象的一个具像
   天网恢恢
   逻辑闭包V2
   道和名的信息屏障
   什么是架构设计V3
   一个架构设计模糊精确的例子
   硬编码Tag方案
   设计语言和编码语言的区别
   用Qemu调试Linux内核的技巧总结
   什么是架构设计V4
   软硬件结合设计的实践问题
   信心和建模问题
   在语义上评价逻辑
   细节迷信
   接口对象问题
   设计的驱动力问题
   什么是架构设计2023
   抽象思维
   架构设计和一般设计的区别
   为什么架构设计必须使用自然语言
   目标约束和实施约束
   专利思维和设计思维
   为什么很多人看书学不会架构设计
   对卷积的感性理解
   为什么不要画市场式的架构图
   不要把细节特征当作设计
   架构设计中猜的成分
   对一个设计评审意见的深入探讨
   关于语义的辨识
   基于状态机的行为定义
   设计问题总结的问题
   高层设计和下层设计的区别V2
   集合分界不同的问题
   一个简单的复杂视图建模例子
   一个设计仿写的例子
   设计的本质
   关于队列模型
   语义纠偏——细节调研的目的和方向
   填空问题
   中文标准写作总结

   一些未分类的例子

.. vim: tw=80 fo+=mM
