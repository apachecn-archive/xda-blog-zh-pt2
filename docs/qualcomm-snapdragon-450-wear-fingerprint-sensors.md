# 高通宣布推出骁龙 450 移动平台、骁龙 Wear 1200 和高通指纹传感器

> 原文：<https://www.xda-developers.com/qualcomm-snapdragon-450-wear-fingerprint-sensors/>

在 2017 年上海世界移动通信大会上，高通发布了其最新的中低端 SoC 骁龙 450 移动平台。新的芯片组比前代产品有许多改进，包括更新的 GPU、改进的相机性能以及更快的调制解调器。

* * *

**骁龙 450**

与骁龙 430 的升级版骁龙 435 不同，骁龙 450 在关键领域进行了一些急需的改进。凭借骁龙 450，高通最终也将 14 纳米制造工艺引入了中端 SoC。我们已经看到了在骁龙 625/626 等芯片中改用 14 纳米工艺的好处，我们迫不及待地想看到它将为中低端智能手机的电池寿命带来的改进。

骁龙 450 使用与骁龙 435 相同的八核 ARM Cortex-A53 实现，所有八个 A53 内核的时钟频率为 1.8GHz。高通声称，与前代产品相比，骁龙 450 的 CPU 和 GPU 性能提高了 25%。CPU 性能的提升部分来自于时钟速度的提升——与之前的 1.4GHz 相比，时钟速度提高了 1.8GHz。尽管时钟速度更高，但骁龙 450 仍然承诺比其前代产品多“多达 4 小时”的使用时间，这要归功于其更高效的 14 纳米工艺。

| 

社会学

 | 

骁龙 450

 | 

骁龙 435

 | 

骁龙 625

 |
| --- | --- | --- | --- |
| **CPU** | 4x A53 @ 1.8GHz4x A53 @ 1.8GHz | 4x A53 @ 1.4GHz4x A53 @ 1.4GHz | 4 个 A53 @ 2.0GHz 4 个 A53 @ 2.0 GHz |
| **内存** | LPDDR3 | LPDDR3 | LPDDR3 |
| **GPU** | 肾上腺素 506 | 肾上腺素 505 | 肾上腺素 506 |
| **编码/解码** | 1080pH.264 & HEVC | 1080pH.264 & HEVC | 1080pH.264 & HEVC |
| **摄像机& ISP** | 双 ISP 13MP + 13MP(双)13MP + 13MP(双)21MP(单) | 双 ISP8MP + 8MP(双)21MP(单) | 双 ISP24MP |
| **调制解调器** | X9 LTE 猫。7 300Mbps 下行链路，150Mbps UL | X9LTE Cat.7 300Mbps DL 100Mbps UL | X9 LTE 猫。7 300Mbps 下行 150Mbps UL |
| **USB** | USB 3.0 w/快速计算器 3.0 | USB 2.0 w/quick harge 3.0 | USB 3.0 w/快速计算器 3.0 |
| **制造过程** | 14 纳米 | 28nm LP | 14 纳米 |
|  |  |  |  |

骁龙 450 上的 GPU 也看到了 Adreno 506 形式的更新，该公司声称比骁龙 435 的 Adreno 505 GPU 快 25%的图形渲染。

骁龙 450 也给相机部门带来了巨大的改进。它现在支持实时散景效果，还包括高通 Hexagon DSP，可带来改进的多媒体、相机和传感器处理，同时仍然使用低功耗。与其前代产品类似，骁龙 450 支持高达 21MP 的单摄像头。然而，当用于双摄像头设置时，它现在可以处理 13MP + 13MP 传感器，比骁龙 435 的 8MP + 8MP 支持有所跳跃。最后，视频处理器也得到了改进，因此骁龙 450 现在可以捕获和播放高达 1080p60 的视频，而骁龙 435 的视频分辨率为 1080p30。很高兴看到这些功能正在向“下游”发展，但这还不是全部:

骁龙 450 支持快速充电 3.0，该公司声称可以在短短 35 分钟内将设备从零充电到 80%——尽管“可以”与“将”截然不同，因为我们看到的实现达不到这一标准。该芯片组还支持 USB 3.0 标准，如果原始设备制造商正确实现这一功能，与骁龙 450 设备相比，这将大大加快数据传输速度。

至于连接，骁龙 450 使用了与前代相同的 X9 LTE 调制解调器，但现在可以达到更快的上传速度。骁龙 450 包括 X9 LTE 调制解调器，支持 LTE 类别 7 和类别 13，下载和上传速度分别高达 300 Mbps 和 150 Mbps。

高通计划在今年第三季度**开始对骁龙进行商业采样，预计该芯片将于 2017 年底**投入使用。

* * *

**骁龙穿 1200**

高通在上海 MWC 发布了一款名为骁龙 Wear 1200 的新型可穿戴芯片组，该公司声称该芯片组将帮助制造商制造超低功耗的可穿戴设备。

高通表示，Wear 1200 将使制造商能够为一系列全新的用例扩展他们的设备，因为新芯片提供了很高的效率和强大的连接功能。Wear 1200 的目标是建立高效、始终连接和经济高效的可穿戴设备，但不是最强大的。

骁龙 Wear 1200 配备了单核 ARM Cortex A7 单核 1.3 GHz CPU，搭配简单的显示控制器。然而，骁龙 Wear 1200 的主要亮点是其新的调制解调器，它增加了对 LTE 类别 M1 和类别 NB1 的支持。新的调制解调器支持上述 LTE 标准上的超低功耗通信模式，也是第一个支持 3GPP 低功耗 WAN 技术的调制解调器。

在连接方面，Wear 1200 支持 Wi-Fi、蓝牙 4.2 LE、LTE 语音和 GPS。

Wear 1200 还提供集成的基于硬件的安全功能，如高通安全执行环境、硬件加密引擎、硬件随机数生成器和 TrustZone，以提供增强的隐私和安全保护。

虽然 Wear 1200 显然不是为智能手表设计的，但你可以期待新芯片为各种可穿戴设备提供动力，从宠物和老人的追踪器到健身带。

骁龙 Wear 1200 现已上市，并将于今日开始发货。

* * *

**高通指纹传感器**

高通在移动半导体行业已经是一个响当当的名字，现在该公司正计划进入指纹扫描仪业务。在 2017 年 MWC 上，这家总部位于美国的芯片制造商发布了下一代**超声波指纹扫描仪，引入了高通指纹传感器**。

大多数原始设备制造商一直在他们的设备上使用电容式指纹扫描仪。然而，如果这个来自高通的新声明是可靠的话，我们将在这方面看到一些巨大的进步。

新的解决方案利用超声波扫描，**将使智能手机原始设备制造商能够在显示器、玻璃或金属下实施指纹传感器**。高通表示，其指纹传感器也可以检测心率和血流量，甚至可以在水下工作。

说到用于显示的高通指纹传感器，该扫描仪允许原始设备制造商在显示面板下实施指纹扫描仪。然而，这种解决方案只能在有机发光二极管面板上使用，液晶面板就没那么幸运了。另一方面，用于玻璃和金属的高通指纹传感器使得在玻璃或金属下实现指纹扫描仪成为可能，并且可以扫描高达 800 米的覆盖玻璃和高达 650 米的铝。

用于玻璃和金属的高通指纹传感器将与骁龙 660 和 630 芯片组兼容。

显示器用高通指纹传感器将于 2017 年第四季度向原始设备制造商提供测试。另一方面，用于玻璃和金属的高通指纹传感器将于本月晚些时候向原始设备制造商提供，预计这些传感器将于 2018 年上半年进入商业设备。

* * *

[**出处①:高通**](https://www.qualcomm.com/news/releases/2017/06/28/qualcomm-snapdragon-450-mobile-platform-bring-14nm-finfet-process-enhanced)