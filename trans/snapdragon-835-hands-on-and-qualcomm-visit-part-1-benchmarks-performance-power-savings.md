# Snapdragon 835 实践和高通访问第 1 部分:基准测试、性能和节能

> 原文：<https://www.xda-developers.com/snapdragon-835-hands-on-and-qualcomm-visit-part-1-benchmarks-performance-power-savings/>

上周，我们受邀前往高通位于加州圣地亚哥的总部，亲眼一睹 Snapdragon 835 的风采。

我们能够测试该公司即将推出的芯片组，并通过与项目负责人交谈和参观庞大的高通办公室来了解其产品设计和理念，以更多地了解他们的相机技术、虚拟现实进步以及他们优化能效的方式。这是一次有趣的旅行，让我们感受到 Snapdragon 835 在今年 4 月及以后的设备中的表现，我们还了解到一些关于该公司试图通过这种新处理器实现什么的额外信息；他们试图向原始设备制造商和消费者推销哪些新功能，以及他们打算如何推广这些新功能。

虽然此行的核心是围绕 Snapdragon 835 的基准测试，但高通强调了一个观点，即太多的移动发烧友只关注同比性能增长，从而只见树木，不见森林。不可否认，他们想要传达的大部分内容很难测量和量化，用真实世界的例子更难有意义地传达。尽管如此，我们将在接触到您可能会发现本文最有趣的部分:基准之后，回顾一下我们学到的一些东西。

| 

规范

 | 

高通骁龙 835

 | 

高通骁龙 820

 |
| --- | --- | --- |
| 芯片集 | 835(10 纳米 LPE) | 821(14 纳米 LPP) |
| 中央处理器 | 4x 2.45GHz 低温 280(大)，4x 1.9GHz 低温 280(小) | 2 个 2.15GHz Kryo，2 个 2.19GHz Kryo |
| 国家政治保卫局。参见 OGPU | Adreno 540 GPU | Adreno 530 GPU，653MHz |
| 记忆 | 2 个 1866MHz 32 位 LPDDR4X | 2 个 1866MHz 32 位 LPDDR4 |
| ip 摄像机 | 双 14 位光谱 ISP 14 位 32MP | 双通道 14 位光谱 ISP 25MP |
| 调制解调器 | 骁龙 X16 LTE(16 类下行链路，13 类上行链路) | 骁龙 X12 LTE(第 12 类下行链路，第 13 类上行链路) |

随着今年早些时候 Snapdragon 835 的正式发布，我们终于通过高通提供的官方数据了解到新处理器相对于 Snapdragon 820 和 821 的同比增长。三星很快就吹嘘了他们新的 10 纳米 FinFET 工艺实现的性能提升——在相同的功耗下，性能提高了 27%,或在类似的性能水平下功耗降低了 40%,而高通的数字略低，CPU 和 GPU 同比提高了 25%。这是一个惊喜，因为传统上，高通自己已经引用了更高的旗舰级发布性能的比例跃升。

让我们通过与之前的数据进行比较来透视一下——以 Adreno GPU 为例。 据报道，骁龙 805 比 800 和 801 中的 Adreno 330 快 40%，而 Snapdragon 810 中的 Adreno 430 进一步将性能提高了 30%。Snapdragon 820 和 821 上的 Adreno 530(具有不同的时钟速度)比上一代产品提供了高达 40%的图形性能。现在，所有这些成比例的增长并不总是直接转化为同样更高的基准测试结果，高通通过这一稳定的 GPU 产品组合一直保持在图形游戏的顶端。但它回避了一个问题，到底为什么高通声称这一代人只有 25%的比例？虽然我们已经了解到新的 Adreno 版本只是一个相当轻微的版本，但 CPU 本身看到了一个新的架构，通过许可协议为基于 ARM 的“半定制”核心放弃了 Kryo 核心，这使得高通部分的修改非常有限(在活动中，他们仍然不愿意确认新的 CPU 是基于 A72 还是 A73 核心)。那么，我们实际上可以从这种芯片组中获得什么样的收益呢？

我们有机会对 Snapdragon 835 进行了短短两个小时的测试，这足以让我们勤奋地测试各种基准，包括 Geekbench 4、3DMark、GFXBench、Basemark OS II、PCMark 和 AnTuTu，同时还允许设备在运行之间合理地冷却，以便为独立运行收集更好的样本。发现处理器的设备是一个不起眼的轻质塑料平板手机，具有磨砂机身，顶级的规格确保尽可能少的瓶颈。根据下表，这些包括 1440p 显示屏、6gb 的 DDR4 RAM 和快速 UFS 存储——虽然高通不能在现场透露他们在这里采用的具体解决方案，但从我使用 Androbench 能够实现的读写速度来看，最肯定的是 UFS 2.1。

| 

设备

 | 

高通测试装置

 |
| --- | --- |
| 模型 | MSM8998 |
| 安卓版本 | 7.1.1 |
| 解决 | 1400 x 2560 |
| 照相机 | 2140 万像素/130 万像素 |
| 随机存取存储 | 6GB |
| 储存；储备 | 64GB UFS (2.1?) |
| 频率范围 | 300-2457.6 兆赫 |

在我们跳到数字之前，我想指出一些解释这些结果时需要知道的警告:骁龙 821 和麒麟 960 的数字是通过更高采样的更好控制的测试获得的，而有限的时间只允许我们在每个基准测试中收集三到八个样本。测试设备上的软件也不稳定，经常决定开始产生可怕的结果，直到重新启动(高通建议我们这样做，因为他们指出这是一个错误)。我们在整个测试过程中监控 CPU 频率，没有发现任何异常，这让我们可以推断没有作弊。最后，这款设备具有出色的热性能，通过我们的前视红外热像仪测量，峰值约为 33°C(91°F)。我们希望我们可以做更仔细的测试，一旦我们拿到实际设备，我们肯定会更深入地研究 835。

从 Geekbench 4 下的 CPU 性能开始，测试设备在 8 次独立运行中设法获得了多核的平均分数 **6403** 和单核的平均分数 **2040** ，最高分是多核的平均分数 **6461** 和单核的平均分数 **2067** 。这是对骁龙 821 的重大改进，不仅高于我们在博客上看到的所谓泄露的基准，也高于 25%的平均水平。作为参考，我们的 OnePlus 3T ( [没有基准测试作弊](https://www.xda-developers.com/benchmark-cheating-strikes-back-how-oneplus-and-others-got-caught-red-handed-and-what-theyve-done-about-it/))，多核平均得分为 4344，单核平均得分为 1828。这意味着我们看到多核处理器的性能提升超过 **45%，但单核处理器**的性能提升仅**略高于 10%。然而，这里有几件事需要考虑:骁龙 835 有一个非对称大的八核芯片。几乎没有设置，而 821 和 Kryo 专注于更少但更强大的对称内核。**

多核的年同比改进看起来很大，主要受益于多线程使用场景，同时仍然为依赖单核的应用程序提供了可观的性能。令人惊讶的是，这些分数也高于我们在华为 Mate 9(设置为“性能”)中为麒麟 960 获得的数字，单核和多核分数都高出不到 5%。Geekbench 4 本身是 CPU 性能的较好预测器之一，因此这些结果本身就很有启发性，也提供了更多关于 Snapdragon 835 CPU 架构的线索。

我们在 GPU 部门发现了一个类似的故事，1080p Manhattan Offscreen (ES 3.1)的输出结果高于我们对高通官方数据的预期。该设备比我们在谷歌 Pixel XL 上获得的分数同比提高了 **33%，比麒麟 960** (Mate 9)中 G71 的帧率高出**50%以上。其他测试也显示了类似的增益，包括 3DMark Slingshot Unlimited 3.1(与分辨率无关)，我们发现它比谷歌 Pixel XL 高出 40%，比华为 Mate 9 高出 60%。测试中的最小和最大帧时间出现了健康的变化，最小帧时间在 1080p 曼哈顿，详尽的汽车追逐基准低于 16.66 毫秒的目标。**

更全面和全面的测试也使 Snapdragon 835 遥遥领先，尽管我们会忽略 PCMark 等测试，因为它们依赖于系统优化，以及我们在几十种不同设备共享同一芯片组时看到的巨大差异。像 Geekbench 4 这样的基准测试，通过使用 NDK 和绕过解释语言开销而更接近金属，应该足以让我们知道我们可以从这些新处理器中期待什么样的数据处理改进。

我还想提醒我们的读者，这些设备是专门为基准测试而提供给我们的**，硬件具有我在智能手机上见过的一些最佳散热特性，因此这些结果很可能会因其实施而异，并且随着时间的推移，性能和其他指标也将与我们在这里遇到的任何东西有很大不同。**

* * *

在与各种高通代表和 SoC 开发负责人交谈时，我发现他们谈话要点的潜在模式围绕着**能效**。例如，高级主管 Travis Lenier 向我解释说，电源效率是 Snapdragon 835 的核心目标，虽然他们可以在其配置下推动更高的性能，但他们认为他们已经取得了平衡，应该支持电池效率的年度改善略高于年度性能改善。

我还怀疑，高通保守的(在上下文中)年度改进数字的一部分来自于这样一个事实，即 Snapdragon 835 的 CPU 和 GPU 的许多增强功能，如更好的分支预测或图形深度拒绝，并没有真正在大多数工作负载上表现出来——一些较小的附加功能，如用于效率集群的更大的 L2 缓存，对现实世界用户体验的改善也比人们用基准测试衡量的要大得多。高通最终相信，他们专注的领域，如虚拟现实，可以节省非常可观的电池寿命。

在我们的访问中，我们设法看到了这样的例子，我们看到骁龙 821 和 Snapdragon 835 正在进行功耗测试([使用您自己可以获得的工具](https://www.msoon.com/LabEquipment/PowerMonitor/))，同时实时运行几个演示。这个装置让我们看到了 821 和 835 在完全相同的工作负荷下电流消耗是如何变化的。在虚拟现实演示中，我们看到了 32%的电流摄入差异，这是一个巨大的增量，也带来了类似的性能提升-其中许多改进也不是来自 GPU，而是 835 中的传感器数据处理和特定的 VR 优化。在一个非常简单的相机演示过程中，差异仍然是可观的 27%，尽管相机是固定的，指向一个没有实际活动的角落，所以我们没有机会移动设置。

* * *

这总结了我们 Snapdragon 835 覆盖范围的第一部分，在下一部分中，我们将重点关注基准无法测量的所有方面，但会影响您的用户体验(通常超出性能)。和往常一样，请记住**高于**的数字并不一定意味着运行 Snapdragon 835 的智能手机将提供出色的性能，尽管我们当然希望它们会如此。

此外，随着 CPU 架构的变化，高通在 821 中提供的一些增强现实性能的功能，如由打开的应用程序和其他用户输入触发的升压模式(CPU 最大化)，将不会在这种新的芯片组中实现。这是可以理解的，因为这是一个非常不对称的芯片组，特别是特定的功能不会像在同构内核的四核芯片组上那样工作。

但正如我们所说，高通正在用 Snapdragon 835 做的许多事情是基准测试无法捕捉到的，在一个小房间里用公司提供的测试单元进行两个小时的基准测试肯定不会告诉我们所有的答案。在未来的后续文章中，我们将讨论整体封装如何提供比原始性能和节能改进更多的功能，以及高通在市场中的地位如何特别要求它们提供超过时钟速度和内核数量的价值。