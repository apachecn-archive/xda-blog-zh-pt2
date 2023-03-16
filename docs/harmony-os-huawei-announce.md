# 华为正式发布其第一款第三方操作系统鸿蒙系统

> 原文：<https://www.xda-developers.com/harmony-os-huawei-announce/>

在中国东莞市，华为终于揭开了传闻已久的第一方操作系统的面纱。这款名为“鸿蒙系统”的操作系统已经开发了好几年，但自从美国对华为颁布贸易禁令以来，它最近在华为的应急计划中扮演了一个关键角色。在华为开发者大会上，华为终于分享了其内部操作系统的第一批细节，但该公司还没有准备好在智能手机上展示 Harmony。明天，该公司将在荣誉电视上展示鸿蒙系统。目前，Android 仍然是华为的首选移动操作系统，也是智能手机和平板电脑的首选。

鸿蒙系统是基于微内核的，就像谷歌正在开发的 Fuchsia OS 一样。华为表示，Fuchsia 采用了“非分布式设计”，不同于新款鸿蒙系统。华为表示，这允许在各种设备上灵活部署新的操作系统，在所有场景下简化应用程序开发。为了证明这两种说法，华为提出，“在 Android 和 Linux 内核中有大量代码的情况下，很难在不同设备上提供流畅的体验。”这是因为“多设备互联[提高了]安全要求”和“应用生态系统和硬件之间的紧密耦合损害了用户体验和开发效率。”

据华为称，使用微内核也提高了安全性。微内核只“提供最基本的服务，如线程调度和 IPC”，而大多数系统服务是在用户空间实现的。由于要审计的代码更少，发现新攻击的概率将会更低。华为还表示，它正在使用“正式的验证方法”来保护 TEE 内核。华为表示，这项技术使用“数学方法从源头验证系统正确性”，主要应用于航空航天和芯片组等安全关键领域，“极大地促进了系统的可靠性和鲁棒性。”此外，微内核可以“根据更广泛的系统安全性的需求进行扩展”最后，华为夸口说，运行新操作系统的产品可以达到 EAL 5+认证水平。

根据华为分享的幻灯片，理论上性能优于 Android 和其他基于 Linux 的操作系统。华为表示，鸿蒙系统使用简化协议的分布式虚拟总线:协议栈中只有一层，而不是 4 层，以“提高有效载荷效率”这种简化交互的变化的效果是“更快地发现和连接”显示器、摄像头、扬声器等硬件。

与使用 Linux 内核调度机制的 Android 不同，鸿蒙系统使用“确定性延迟引擎”，提供“精确的资源调度，实时负载分析和预测以及应用程序特征匹配”结果是响应延迟和延迟波动分别提高了 25.7%和 55.6%。此外，华为表示，微内核可以使“IPC[进程间通信]性能的效率比现有系统高五倍”，特别是指谷歌的 Fuchsia OS。

Harmony 将操作系统与硬件“解耦”,因此开发人员可以一次开发并跨硬件部署。开发者将能够使用华为的 ARK 编译器为鸿蒙系统编译多种语言的代码，如 C/C++、Java 和 Kotlin。华为将提供一个 IDE 来支持多种设备类型的应用开发，包括电视、车载套件、智能扬声器、智能手机、智能手表等。这个 IDE“自动适应不同的屏幕布局、控件和交互”，并且“支持拖放操作和面向预览的可视化编程”鸿蒙系统不需要 root 用户权限就能运行，华为称这在 Android 和其他基于 Linux 的操作系统上是一个安全风险。最后，华为宣布了其开源鸿蒙系统、建立开源基金会和创建开源协作社区的计划。

华为消费者业务集团首席执行官 Richard Yu 证实，鸿蒙系统与开箱即用的 Android 应用程序不兼容。这意味着你不能简单地下载你选择的任何安卓应用。在一次新闻发布会上，俞敏洪表示，应用程序开发者必须对他们的应用程序进行“小改动”，才能编译成能在鸿蒙系统上运行的程序。他表示，将安卓应用转移到鸿蒙系统“非常容易”。

新操作系统的工作始于两年前的 1.0 版本的微内核。2019 年，他们加快了工作速度，以便操作系统可以在更多类型的设备上工作，如智能屏幕产品。这家中国公司表示，其微内核的 2.0 版本将于明年发布，而 3.0 版本将于 2021 年发布，为可穿戴设备和汽车头部单元提供支持。华为表示，他们现在可以切换到鸿蒙系统，因为由于微内核的性质，迁移并不十分困难；他们吹嘘他们可以在 1-2 天内从 Android 切换到 Harmony。然而，该公司目前选择在智能手机上坚持使用 Android，而不是考虑其现有的合作伙伴。Richard Yu 表示，华为希望继续与美国合作伙伴合作并为其提供帮助，其中许多合作伙伴已经与华为合作了 20 多年。

然而，这个新的操作系统仍然是中国科技巨头的“B 计划”，因为华为需要解决采用鸿蒙系统的最大漏洞:应用生态系统。华为正在建立其 AppGallery 平台，作为谷歌 Play 商店的替代产品，本周该公司推出了华为移动服务，作为 Google Play 服务的替代产品。华为正在建立自己的生态系统，如果贸易禁令在今年年底或明年年初没有解除，那么华为将被迫转向鸿蒙系统购买其新设备，包括即将推出的华为 Mate 30 系列。事实上，Richard Yu 证实，Mate 30 在贸易禁令颁布前没有获得使用 Google Play 服务的认证，因此如果禁令没有及时解除，华为正在考虑在该设备上使用鸿蒙系统。

华为表示，其新操作系统代表了全新一代的操作系统，因为它能够在不同于 PC、平板电脑和其他领域的不同场景中实现人工智能能力。华为已经在多种设备上对其新操作系统进行了内部测试，但 Richard Yu 没有确认可折叠的华为 Mate X 是否在这些测试设备中。俞敏洪表示，“许多”合作伙伴都表示有兴趣与鸿蒙系统合作开发产品，但他拒绝透露感兴趣的公司名称。在一份新闻稿中，华为表示，他们将首先“为鸿蒙系统在中国市场奠定基础”，然后再将其扩展到全球市场。

我们将在本周的华为开发者大会上了解更多关于华为新操作系统的信息。

* * *

*美国东部时间 2019 年 8 月 10 日上午 10:23 更新:措辞已更改，以反映鸿蒙系统不要求 root 用户访问权限才能运行，而不是不允许。还澄清了 5 倍 IPC 性能是对谷歌的 Fuchsia。*