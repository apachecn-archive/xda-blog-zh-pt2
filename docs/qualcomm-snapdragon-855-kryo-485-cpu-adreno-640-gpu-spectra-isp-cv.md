# 高通骁龙 855:CPU、GPU、ISP 和 DSP 概述

> 原文：<https://www.xda-developers.com/qualcomm-snapdragon-855-kryo-485-cpu-adreno-640-gpu-spectra-isp-cv/>

高通在今年的骁龙科技峰会上正式开始详细介绍其下一代骁龙 855 移动平台。[昨天宣布，](https://www.xda-developers.com/qualcomm-snapdragon-855-snapdragon-elite-gaming-3d-sonic-sensor/)高通最新的移动平台预计将成为 2019 年最多产的旗舰智能手机的核心，现在我们能够一窥高通最新最伟大的设计提供了什么。这是我们目前所知的。

* * *

#### 鸟瞰图

凭借骁龙 855，高通再次专注于五大核心支柱:**性能、人工智能、相机、娱乐，当然还有连接性**。虽然高通一直处于连接的前沿，特别是随着 5G 的到来，该公司可以充分利用其最近的投资，利用[骁龙 X50 调制解调器](https://www.xda-developers.com/qualcomm-snapdragon-855-sdx50-5g-modem/)利用毫米波频段。高通骁龙 855 还升级了两个对现代智能手机体验越来越重要的组件:[Hexagon DSP](https://www.xda-developers.com/qualcomm-snapdragon-845-hexagon-685-dsp/)和 Spectra ISP。前者处理图像和传感器数据，并帮助人工智能计算。然而，Spectra ISP 已经使许多高通驱动的旗舰设备保持在移动摄影的前沿，这个特殊的组件正在经历其最大的升级之一，我们将在另一篇文章[中进一步详细介绍。](https://www.xda-developers.com/qualcomm-spectra-380-isp-integrated-ai/)

最后，还有 CPU 和 GPU 性能的核心改进，高通一直在稳步和可观地逐年提高。骁龙 855 引入了基于 ARM 最新内核设计的新 Kryo 485 CPU 内核，以及 Adreno 640 GPU，实现了一流的游戏性能，正如我们所期待的那样，高通在这方面一直保持着优势。采用 TSMC 最新的 7 纳米 FinFET 工艺制造，我们可以在所有移动工作负载中实现高性能和节能。这些改进使 CPU 性能提升了 45%，GPU 速度提升了 20%。

|  | **高通骁龙 855** | **高通骁龙 845** |
| **CPU** | 1 Kryo 485‘Prime’(基于 A76)，高达 2.84GHz 3 Kryo 485(基于 A76)，高达 2.42GHz 4 Kryo 385(基于 A55)，高达 1.8GHz 比上一代性能提升 45% * | 4 Kryo 385(基于 A75)，提升 2.8GHz 4 Kryo 385(基于 A55)，提升 1.8GHz 比上一代性能提升 25% * |
| **GPU** | Adreno 640 比上一代产品性能提升 20% * | Adreno 630 比上一代产品性能提升 25% * |
| **内存** | 4x 16 位 2133MHz LPDDR4X | 4x 16 位 1866MHz LPDDR4X |
| **ISP** | 双 14 位 Spectra 380 ISP 48MP 单摄像头，22MP 双摄像头 4K 60FPS HDR 视频带实时物体分割(人像模式，背景互换) | 双 14 位 Spectra 280 ISP 32MP 单摄像头，16MP 双摄像头 4K 60FPS HDR 视频 |
| **调制解调器** | 骁龙 X24 LTE 2000Mbps DL(目录。20)、316Mbps UL (Cat 20) 骁龙 X50 (5G 调制解调器)5000 Mbps DL | 骁龙 X20 LTE 1200Mbps DL (Cat。18)，150 兆位/秒 UL(第 13 类)。 |
| **制造工艺** | 7 纳米(TSMC) | 10 纳米 LPP(三星) |

*基于高通在各自发布时提供的数字。

### 完整的功能列表-单击以展开

**高通人工智能引擎**

*   高通 Hexagon 690 处理器
*   高通 Adreno 640 GPU
*   高通 Kryo 485 CPU

**连通性**

*   骁龙 X24 LTE 调制解调器 LTE 类别 20
*   骁龙 X50 5G 调制解调器(用于 5G 设备)
*   高通 Wi-Fi 6-ready 移动平台:802.11ax-ready、802.11ac Wave 2、802.11a/b/g/n
*   高通 60 GHz Wi-Fi 移动平台:802.11ay，802.11ad
*   蓝牙版本:5.0
*   蓝牙速度:2 Mbps
*   双频 GNSS 高精度定位

**高通 Spectra 380 图像信号处理器**

*   双通道 14 位 CV-ISPs；22MP @30 fps 并发双摄像头；48MP @ 30 fps 单摄像头
*   硬件 CV 功能包括对象检测和跟踪(梯度方向直方图、哈里斯角检测、归一化互相关、线性分类和光流)以及立体深度处理
*   先进的 HDR 解决方案，包括改进的 zzHDR 和 3 曝光四色滤光片阵列(QCFA) HDR
*   4K60 HDR 视频拍摄(HDR10、HDR10+和 HLG)，支持人像模式(散景)、10 位色深和 Rec。2020 色域
*   用于快照的基于硬件的多帧降噪(MFNR)和用于视频的运动补偿时间噪声滤波(MCTF)
*   相机子系统中基于硬件的电子图像稳定(EIS)解决方案
*   一种新的模块化 ISP 设计，在 RAW 和 YUV 像素域中更灵活地接入和断开成像管道
*   慢动作视频的高帧速率捕捉(720p @ 480fps)
*   HEIF 照片采集，HEVC (H.265)视频采集

**音频**

*   高通声音技术公司
*   高通 aptX 支持，包括经典 aptX、aptX HD 和 aptX adaptive
*   高通 TrueWireless 立体声增强版

**高通肾上腺素视觉子系统**

*   Adreno 640 GPU
*   Vulkan 1.1 API 支持
*   HDR 游戏(10 位色深，rec 2020 色域)
*   基于物理的渲染
*   API 支持:OpenGL ES 3.2，OpenCL 2.0 FP，Vulkan 1.1
*   最大设备显示支持:高达 4K HDR
*   最大外部显示器支持:多达两个 4K HDR 显示器
*   硬件加速的 H.265 和 VP9 解码器
*   支持 HDR10+、HDR10、HLG 和杜比视界的 HDR 回放编解码器
*   体积虚拟现实视频播放
*   8K 360 VR 视频播放

**高通 Kryo 485 CPU**

*   一个主内核时钟速度:高达 2.84GHz
*   三个高性能内核时钟速度:高达 2.42GHz
*   四个高效内核时钟速度:高达 1.80GHz
*   架构:64 位

**流程**

**高通 Hexagon 690 处理器**

*   安全处理能力
*   四线程标量内核
*   四个高通六边形矢量扩展(HVX)
*   高通六边形张量加速器
*   高通六角形语音助手
*   高通全方位感知技术

**安全**

*   高通生物认证套件:指纹、高通虹膜认证、语音、面部、高通安全处理单元，支持移动支付
*   高通三维声波传感器

**高通快充 4+技术**

**内存**

*   内存速度:2133MHz
*   内存类型:4x 16 位，LPDDR4x

* * *

## 组件和功能细分

* * *

## 7 纳米工艺，Kryo 485 CPU 和 Adreno 640 GPU

骁龙 855 是高通首款 7 纳米 FinFET 芯片组，紧随麒麟 980 和苹果 A12 发布，后者是首款商用 7 纳米移动平台。这并不令人惊讶，因为高通传统上选择尖端的工艺尺寸，并且该公司证实他们已经对他们的 7 纳米骁龙旗舰芯片组进行了采样。迁移到 7 纳米能够增加晶体管密度，同时实现**性能和功率效率分别提高 20%和 40%左右**、[，尽管这是与 TSMC 自己的 10 纳米 FinFET 工艺相比而言的](http://www.tsmc.com/english/dedicatedFoundry/technology/7nm.htm)。至于骁龙 855 的 CPU 性能，高通表示，我们应该预计**的性能比骁龙 845** 提高 45%，这是该公司近年来最大的同比性能提升之一。

高通骁龙 855 的八核 CPU 安排还引入了该公司的 **Kryo 485 核心，其时钟频率为 2.42GHz** 用于高性能集群，**为 1.8GHz 用于低功耗集群。**最重要的是，正如传言所言，骁龙 855 正在引入一个时钟高达 2.84Ghz 的**‘prime’集群**。Kryo 485 是一种半定制的核心设计，与系统架构相一致，同时提供一些服务质量优化。金色内核基于 [ARM 的 Cortex-A76 架构](https://www.xda-developers.com/arm-cortex-a76-cpu-mali-g76-gpu-mali-v76-vpu-announcement/)，该架构承诺性能提升高达 35%，能效提升 40%，而银色内核基于 Cortex A55，如骁龙 845 上所见。基于 ARM Cortex 的许可证应该仍然非常有限，但考虑到高通提供的数字(以及这些数字如何与过去的性能相吻合)，结果一定很有希望。了解这些内核的基础应该也能让我们对未来有一个很好的认识。

我们还了解了新的 Adreno 640 GPU，以及高通所谓的**“骁龙精英游戏体验”**，这是一套旨在改善骁龙设备上的移动游戏的功能和合作伙伴关系。该公司的新 Adreno 640 GPU 保持领先地位，与去年的骁龙 845 中的 Adreno 630 相比，性能提升了 20%。虽然 Adreno 系列已经提供了许多代的顶级性能，但也值得注意的是，我们可以期待 Adreno 640 继续保持领先的性能功耗比。Adreno 640 的算术逻辑单元(ALU)增加了 50%，应该可以进一步提高人工智能工作负载的性能。

高通意识到手机游戏越来越受欢迎，特别是在印度和中国等地区，但也是因为像堡垒之夜和 T2 这样广受好评的游戏的到来。正因为如此，该公司正与游戏引擎开发商以及游戏工作室密切合作，以确保流行游戏针对骁龙设备进行优化。此外，高通和 Unity 正在寻求简化移动游戏从**到基于物理的渲染(PBR)的过渡，**将视频游戏图形的真实性提升到一个新的水平。最后，虽然 Snapdragon 835 和骁龙 845(分别)允许播放和捕捉 10 位真正的 HDR 视频，但**骁龙 855 将是第一个允许真正的 HDR 游戏的移动芯片组**。[在骁龙 675](https://www.xda-developers.com/qualcomm-snapdragon-675-chipset/) 中，高通引入了一种“定制算法”，他们声称**可以将游戏中的丢帧率降低高达 90%——**虽然我们对这一功能还知之甚少，但骁龙 855 也将实现这一功能。所有这些加上 [Vulkan 1.1](https://www.xda-developers.com/khronos-group-vulkan-1-1-specs/) 支持和 Kryo 485 上看到的改进应该会导致游戏性能的显著增强。

* * *

## Spectra 380 ISP-CV，Hexagon 690 DSP 和 5G

这款**Sp****electra 380 ISP**为高通骁龙 855 带来了一些最重要的改进，该公司称其为**第一款移动 CV-ISP**(CV 代表计算机视觉)。在一次媒体吹风会上，高通的代表解释说，该 ISP 借用 CPU、GPU 和 DSP 的计算单元来帮助计算机视觉任务，并将它们直接放在模块上，以释放其他组件的周期，同时提高性能和可用马力。由于集成的硬件加速 CV 功能，Spectra 380 可以在对象分类、对象分割和深度感测方面提供**改进的性能，同时看到**高达 75%的节能**。由于这些进步，我们可以期待新的**功能，如散景视频**，以及世界上第一个具有肖像模式**或背景交换的 **4K HDR 视频捕捉，以及 **HDR10+视频捕捉**。摄影也将从改进的对象分割中受益，实现实时背景交换和更好的人像模式拍摄。**

虽然该公司没有明确引入“神经处理单元”，但人工智能工作负载也将受益于新改进的 **Hexagon 690 DSP** ，**将矢量加速器(HVX)** 的数量从两个增加到四个，与四个标量线程协同工作。最重要的是，Hexagon 690 带来了第一个移动张量加速器 **Hexagon 张量加速器(HTA)** 。DSP 的改进应该转化为**改进的语音助手性能**从热门词汇检测到设备上的命令解析，例如提供改进的回声消除和噪声抑制。高通强调，他们提供了一个完整的异构计算平台，允许人工智能工作负载接入 CPU、GPU 或 DSP，或者这三个模块的任何组合。“**高通人工智能引擎”**也超越了硬件，因为我们还找到了对骁龙神经处理 SDK 和 Hexagon NN 访问前述模块的支持，以及 Android NN API 和流行的 ML 框架，如 Caffe/Caffe 2、TensorFlow/Lite 和 ONNX(开放神经网络交换)。要了解关于 Hexagon DSP 的更多信息，[请查看去年的文章，详细介绍它如何帮助处理人工智能工作负载](https://www.xda-developers.com/qualcomm-snapdragon-845-hexagon-685-dsp/)。

最后，谈到连接，骁龙 855 是高通的“千兆一切”芯片组。骁龙 855 封装了**世界上第一个 Wi-Fi6 11ax 就绪移动解决方案**，具有 8x8 声音等功能，以高效地为更多设备提供服务，具有 [WPA3](https://www.xda-developers.com/wpa3-wifi-security-standard-final-snapdragon-845/) 的最新安全性，以及高达 67%的更高能效。此外，它还支持**60g Hz Wi-Fi**，基于 [802.11ay 的平台](https://www.xda-developers.com/qualcomms-next-gen-60ghz-wifi-chips-will-deliver-10gbps-speeds/)采用 **Wi-Fi，速度高达 10Gbps** ，延迟甚至更低。正如新的高通芯片组所预期的那样，骁龙 855 通过骁龙 X24 LTE 调制解调器将数据连接速度提高了高达 **2Gbps Cat 20 LTE。因此，[骁龙 X24](https://www.xda-developers.com/qualcomm-x24-modem/) 调制解调器通过 4x4 MIMO 在五个聚合 LTE 载波上提供两倍于上一代 LTE 调制解调器的峰值下载速度，并支持高达 316 Mbps 的 **Cat 20 上传速度**。最重要的是，原始设备制造商还可以选择**骁龙 X50 5G 调制解调器**，支持 sub-6GHz 和毫米波频段，**下载速度高达 5Gbps，延迟前所未有**。高通声称，在毫米波频段，与目前的商业解决方案相比，用户可以预期平均性能快 20 倍。当然，鉴于 5G 网络的部署速度，后者在发布时不会产生太大影响。例如，威瑞森已经在四个城市有限地推出了 5G(有限的下载速度约为 300Mbps)，但整个世界将不得不等待更长时间才能利用这些连接改善。要了解更多关于 2019 年 5G 部署的计划，请查看我们昨天的文章。**

* * *

像往常一样，你可以预计骁龙 855 将成为 2019 年最高产的设备之一——特别是考虑到高通在 5G 连接方面的优势，以及多家原始设备制造商已经取笑或宣布明年支持 5G 的设备。2018 年骁龙科技峰会还远未结束，关于高通骁龙 855 还有很多需要了解的。点击这里查看我们关于骁龙 855 最新变化的更深入的文章。更多信息，请继续关注 XDA 开发者，因为本周我们将有更多骁龙 855 的新闻和内容。