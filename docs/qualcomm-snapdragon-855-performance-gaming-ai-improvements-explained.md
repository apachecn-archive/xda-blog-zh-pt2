# 高通如何改进骁龙 855 的性能、游戏和人工智能

> 原文：<https://www.xda-developers.com/qualcomm-snapdragon-855-performance-gaming-ai-improvements-explained/>

在 2018 年高通骁龙峰会上，该公司[宣布了他们最新的顶级旗舰芯片组:骁龙 855 平台](https://www.xda-developers.com/qualcomm-snapdragon-855-snapdragon-elite-gaming-3d-sonic-sensor/)。这款新产品将成为 2019 年大多数多产旗舰的核心，通过骁龙 X50 调制解调器带来令人难以置信的数据速度。然而，除此之外，骁龙 855 为每个片上系统带来了一系列改进，一些计算单元的性能和能效提高幅度是近年来最大的。

[例如，我们已经详细介绍了 Spectra 380 ISP-CV](http://www.xda-developers.com/qualcomm-spectra-380-isp-integrated-ai) ，它进一步改善了智能手机的拍照效果，同时也为用户节省了大量电池。虽然我们越来越关注外围组件，如 Hexagon DSP，但发烧友最关注的核心模块——即 CPU 和 GPU——也在架构改进和迁移到新的处理节点方面取得了不小的进步。在这篇文章中，我们将快速概述骁龙 855 的 CPU、GPU 和 DSP 的新功能和已知功能，以及这些改进和新功能如何在 2019 年影响*您的*用户体验。

* * *

## 基于 A76 的 Kryo 485 CPU 和向 7 纳米的迁移

骁龙 855 转向 TSMC 最新的 7 纳米 FinFET 制造工艺。我们通常每一两年就会看到一次节点修订，包括尺寸缩小或周期中期优化(如三星 LSI 节点从“低功耗早期”(LPE)到“低功耗增强”(LPP)，所以你可能在某篇新闻文章中听说过这些指标。但这意味着什么呢？在这种情况下，它描述了处理器晶体管特性的大小，这反过来又为我们提供了每一代新处理器的晶体管密度改进的线索。随着每单位面积上更多的晶体管，处理器的最终性能可以按比例提高。这一特性也很重要，因为更小的处理节点允许以更小的规模实现处理器设计，这直观地缩小了处理器元件之间的空间，从而缩短了电子完成计算必须行进的距离。这带来了性能的提升，并且更小的工艺也具有更低的电容，这意味着晶体管可以以更低的延迟和更低的能量开启和关闭。作为参考，TSMC 声称向 7 纳米工艺的转移分别实现了 20%和 40%的性能和功率效率，[，尽管这是与 TSMC 自己的 10 纳米 FinFET 工艺](http://www.tsmc.com/english/dedicatedFoundry/technology/7nm.htm)相比而言的。

在过去的几款骁龙旗舰芯片组中，我们看到高通与三星合作，实施了他们的 14 纳米和 10 纳米 LPP/LPE 工艺。然而，骁龙 855 转向 TSMC 的 7 纳米并不出人意料，因为三星的 7 纳米工艺刚刚在 10 月份进入大规模生产，尽管当时有报道称 5G 高通芯片组将基于此。此外，三星的 7LPP 设计是在一种称为极紫外光刻(EUVL)的改进光刻技术下制造的，与 10 纳米 FinFET 前辈相比，在相同的设计复杂性下，面积减少了 40%，速度加快了 20%，功耗降低了 50%。每一次向更小流程节点的新跳跃都值得庆祝，因为它们是如此难以实现。例如，随着晶体管变得越来越小，它们可能会显示出更大的“泄漏”或流经“关闭”晶体管的电流，从而增加空闲状态下的静态功耗。虽然具有更密集晶体管数量的更小芯片可能允许最大限度地利用给定的硅晶片，但由于前述的泄漏，加上难以获得以其(高)参考频率运行的“更高装箱数”的处理器，产量往往更低。这些只是许多开发障碍中的一些，当新的工艺节点进入大规模生产时，这些障碍当然会被消除，但简而言之，有许多研发和制造挑战会增加将新工艺尺寸推向市场的成本。

为 Kryo 485 授权的最新 ARM A76 架构是我们在高通骁龙 855 上看到的大幅同比改进的另一个重要贡献者。A76 core 是 ARM 奥斯汀办事处的全新白板设计，采用从头开始构建的全新微架构，提供 ARM 所谓的“笔记本电脑级性能和移动效率”它仍然是一个半定制的设计，高通已经做了一些改进，比如优化数据预取以提高效率，以及更大的无序执行窗口。与 A75 相比，这种新设计提供了一些巨大的性能改进，骁龙 845 的黄金内核基于 A75:它承诺性能提高 **35%，能效提高 40%**。当在 750 MW/内核的相同功率包络下，将 10nm 工艺的 A75 与 7nm 工艺的 A76 进行比较时，新内核的性能优势增加到 40%,节能也可以攀升到 50%。此外，非对称单指令多数据(ASIMD)流水线和[点积指令](http://www.linleygroup.com/newsletters/newsletter_detail.php?num=5884)的其他改进将机器学习任务的性能提高了约 3.9 倍，如卷积神经网络中的推理。所有这些都是行业领先的单位面积性能，是对新 7 纳米工艺的巨大补充，高通的 2.84GHz“主内核”接近 ARM [在详细介绍新内核时使用的](https://www.xda-developers.com/arm-cortex-a76-cpu-mali-g76-gpu-mali-v76-vpu-announcement/)3 GHz 参考时钟速度。总而言之，**高通承诺在 845 的基础上实现 45%的 CPU 性能提升**，这是迄今为止最大的同比提升。

说到骁龙 855 的“主核心”，看到高通采用这种新的集群设置也就不足为奇了。ARM 的 [DynamIQ](https://www.xda-developers.com/arms-dynamiq-focuses-on-performance-efficiency-redundancy-scalability-and-latency/) 技术平台很少支持。本质上，DynamIQ 在多核处理器设计中提供了更大的灵活性和可扩展性，允许在给定的集群中进行多核设计，以及细粒度的每核电压控制。(编辑:在一次问答中&答，高通确认主核与性能集群共享其电源域，限制了这里描述的效用)。A76 特别适合这样一个拥有自己时钟的独立优质内核，因为它超越了单线程性能的极限，每时钟整数指令数比 A75 多 25%，ASIMD 和浮点性能高 35%，同时内存带宽高 90%。简而言之，A76 比前几代车型有更大的换代提升，这无疑也有助于高通的骁龙 855 比往常更高的同比性能提升(作为参考，高通引用了 845 比 835 提升 25%至 30%的数据)。这可能足以让高通骁龙 855 的最终性能领先于三星 LSI 在 Exynos 9810 中发现的 mongose 3(M3)内核，尽管这种特殊的设计在功效方面受到了高通芯片没有的影响，骁龙 855 也很可能不会受到影响。

这对最终用户意味着什么？当然，我们应该期待更多的基准内核——ARM 预计移动 Geekbench 得分将提高 Javascript 性能将提高 35%。除了可能与最终用户体验关系不大的基准测试之外，A76 延续了 A75 对**持续性能**的关注，这意味着用户在长时间的游戏会话中应该期望更少的节流。迁移到 7 纳米与新的核心设计相结合，肯定会为最终用户带来显著的电池寿命改善，这可能是这一系列升级最具吸引力的功能。新的“Prime”内核也很有趣，考虑到专注于顶级单线程性能的单个内核可能有利于未设置为充分利用多线程的应用和进程。当然，7 纳米制造工艺还会进一步影响骁龙 855 的其他模块，为日常用户体验中涉及的其他计算单元带来相同的节能效果，例如智能手机摄影的图像处理。

* * *

## “骁龙精英游戏体验”和 Adreno 640 GPU

高通骁龙 855 这次重点关注游戏，鉴于《堡垒之夜》和 PlayerUnknown 的《战地》等游戏的流行以及移动电子竞技在亚洲越来越受欢迎(是的，这是一件事)，这一转变并不令人惊讶。根据高通从 *Newzoo 2017 年全球游戏市场报告*中显示的数字，移动游戏正在上升，预计 2018 年总收入为 703 亿美元，占所有游戏收入的 51%，同比增长 25.5%。

Adreno 640 GPU 为图形性能带来了 20%的健康提升，进一步增强了高通在这一特定领域的竞争优势。不过，作为参考，骁龙 845 比 Snapdragon 835 提升了 30%，Snapdragon 835 本身也比骁龙 821 提升了 30%。不过，这应该会让高通在图形性能方面保持领先，最重要的是，如果他们能够在这方面有所改善，性能功耗比也会保持领先。除了这个数字，高通在谈到 Adreno 时还像以往一样神秘:我们听说了用于电源管理的集成微控制器，以及 640 如何具有最低的驱动程序开销，尽管该公司确实提到了包括多 50%的算术逻辑单元**(ALUs)，这将进一步加快人工智能的性能。**

 **高通在简报会上花了很多时间谈论的一件事是，他们希望将“基于物理的渲染”(PBR)带到更多的移动游戏体验中。PBR 是一种着色模型，允许真实的图形渲染，根据纹理中表示的材质或表面的镶嵌精确地模拟光流。这允许游戏中的对象适当地模仿真实世界材料的视觉属性，包括适当地渲染微表面，如磨损和镜面高光。然而，最显著的改进在于它如何允许更准确地描绘所有表面的反射率和光泽，即使是那些来自平坦和不透明(模拟)材料的表面。

高通和流行的 Unity 引擎背后的开发者一直在努力使 PBR 更容易访问，但该公司也与其他引擎和游戏开发商合作，为骁龙设备优化移动游戏。例如，Unity、Unreal、Messiah 和 NeoX 等游戏引擎已经针对骁龙设备进行了优化，骁龙 855 支持最新的图形 API，如新的 [Vulkan 1.1](https://www.xda-developers.com/khronos-group-vulkan-1-1-specs/) 。NetMarble 是《天堂二:革命》的制作人，像它这样的工作室过去也曾与高通合作，以最好地展示骁龙平台的优势。此外，对于[骁龙 675](https://www.xda-developers.com/qualcomm-snapdragon-675-chipset/) ，我们看到了关于定制算法的讨论，与没有优化的相同平台相比，**实现了多达 90%的 janks** ，同样的变化也出现在骁龙 855 上。目前还不清楚这些优化需要什么，我们也不指望它们适用于每一款游戏，但它肯定意味着更好的性能，至少在 Android 上的大型游戏中。

最重要的是，虽然 Snapdragon 835 和 845(分别)允许回放和捕捉 10 位真正的 HDR 视频，但高通骁龙 855 将是第一个允许真正的 HDR 游戏的移动芯片组。这将需要真正支持 HDR 的显示屏，幸运的是，这在旗舰智能手机中越来越普遍。因此，用户可以期待更丰富的色彩、更深的色调、更高的动态范围(顾名思义)和更高的对比度。这不一定是一个必须具备的功能，但考虑到当前的 HDR 游戏设置需要昂贵的 HDR 电视和显示器，以及功能强大的计算机和特定的游戏控制台，这当然很好。有了高通骁龙 855，游戏中的 HDR 可以说更加容易接近和方便(当然，没有触摸屏控制)。

* * *

## 面向人工智能工作负载的新型 Hexagon 690 DSP

尽管该公司在其营销材料中没有明确称其为“神经处理单元”，但人工智能工作负载也将受益于新改进的 Hexagon 690 DSP。高通在许多代之前就悄悄地推出了这些协处理器(随着 QDSP6 v6 和 820 的适当推出)，但直到最近他们才开始将它们作为人工智能的一些更好的 SoC 模块。DSP 的架构最初是为加速成像工作负载而设计的，特别是包含了六边形矢量扩展(HVX)后，它非常适合 ML 任务。与固定功能硬件相比，DSP 更具可编程性，同时仍保留了特定应用处理器模块的一些性能和效率优势，大大加快了标量和矢量运算的速度。事实证明，这对于不断变化的图像处理算法来说非常出色，这些算法可以卸载到 DSP，但也自然有助于人工智能工作负载。Hexagon DSP 一直是边缘设备上机器学习的[福音，因为它具有出色的硬件级多线程和并行计算能力，能够在每个处理周期处理数千位的矢量单元，相比之下，平均 CPU 内核的每个周期处理数百位，并为多个卸载会话提供服务。](https://www.xda-developers.com/qualcomm-snapdragon-845-hexagon-685-dsp/)

Hexagon DSP 特别适合成像任务，因为它可以绕过设备的 DDR 存储控制器，直接将数据从成像传感器传输到 DSP 的本地存储器(L2 缓存)。例如，谷歌在推出自己的 [Pixel 视觉核心](https://www.xda-developers.com/pixel-visual-core-google-custom-soc/)之前，使用 Hexagon DSP 的图像处理来支持 Pixel 和 Pixel 2 的 HDR+算法。它也是六边形就绪的设备，从流行的谷歌相机端口可以看到最好的结果，你可以在这里探索。它已经被用于虚拟和增强现实工作负载，著名的是在[联想 Phab 2 Pro](https://www.xda-developers.com/project-tango-comes-to-mobile-with-the-lenovo-phab-2-range/) 和[华硕 ZenFone AR](https://www.xda-developers.com/asus-announces-zenfone-ar-and-zenfone-3-zoom-at-ces-2017/) 上驱动[现已解散的](https://www.xda-developers.com/project-tango-dead-google-arcore/)项目 Tango。也就是说，大多数实施骁龙旗舰设备的原始设备制造商以这样或那样的方式利用 Hexagon DSP 进行图像处理，您可以使用[骁龙剖析器](https://developer.qualcomm.com/software/snapdragon-profiler)等工具来验证这一点。

那么，新的 DSP 有什么新特性呢？Hexagon 690 将矢量加速器(HVX)的数量从两个增加到四个，与四个标量线程协同工作，性能也提高了 20%。最重要的是，Hexagon 690 带来了第一款手机张量加速器 **Hexagon 张量加速器(HTA)** 。这是一个重要的补充:它可以作为昂贵的矩阵乘法的硬件加速，还可以在硬件级别集成非线性函数(如 sigmoid 和 ReLU)，进一步加快推理速度。DSP 的这些变化应该会转化为**更好的语音助手性能**，例如，从热词检测到设备上的命令解析，提供改进的回声消除和噪声抑制。高通强调，他们提供了一个完整的异构计算平台，允许人工智能工作负载接入 CPU、GPU 或 DSP，或者这三个模块的任意组合——用高通的加里·布罗特曼的话说，这就是**“不止一个内核，不仅仅是硬件，这是一个完整的系统”**。他们的第四代“高通人工智能引擎”也超越了硬件，因为我们还找到了对骁龙神经处理 SDK 和 Hexagon NN 的支持，以访问上述模块，以及 Android NN API 和流行的 ML 框架，如 Caffe/Caffe 2、TensorFlow/Lite 和 ONNX(开放式神经网络交换)。总之，骁龙 855 可以提供三倍于其前身的原始人工智能性能(是华为的两倍)，超过每秒 7 万亿次运算。但是，请记住，高通继续专注于异构计算解决方案，而不是专注于单个专用模块。

要了解关于 Hexagon DSP 的更多信息，请查看去年的文章，详细介绍它如何帮助处理人工智能工作负载。

* * *

总之，骁龙 855 的计算包带来了近年来我们看到的一些更具影响力的逐年改进。我们在另一篇文章中介绍的 Spectra 380 ISP-CV[也极大地提升了性能和能效，实现了出色的新功能，如 4K 60FPS HDR 视频录制*和*人像模式或背景交换(相当灵活！).](http://www.xda-developers.com/qualcomm-spectra-380-isp-integrated-ai)

正如本文所解释的，这些进步和新特性应该在整个用户体验中被切实地感受到。我们期待着高通骁龙 855，并很快开始深入测试它，所以请继续关注 XDA-开发商的最新骁龙 855 新闻和分析！**