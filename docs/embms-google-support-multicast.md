# 谷歌正在增加对 eMBMS 的支持，以减少移动网络拥塞

> 原文：<https://www.xda-developers.com/embms-google-support-multicast/>

在 AOSP 的最新产品中，谷歌增加了对 eMBMS 的支持。eMBMS 代表演进多媒体广播/组播服务，也被称为 [LTE 广播](https://www.qualcomm.com/invention/technologies/lte/broadcast)。这项技术存在于 Snapdragon 800 系列和更高版本中，谷歌现在正在添加对该服务的全面支持。当许多人可能希望在一个地区或网络中观看或查看相同的内容时，这项服务非常有益。例如，可能使用它的情况是想要广播现场事件的不同角度。不同于向每个用户发送单独的视频流(单播)，相同的视频流同时发送给每个人，并由用户自己选择(多播)。

* * *

## 什么是 eMBMS？

要解释 eMBMS，首先需要解释多播。如上所述，多播是一种在不使其使用的系统过载的情况下一次向不同用户发送视频流的系统。

*eMBMS 演示。安恩特科技的视频。*

这项技术首次亮相于 MSM8974，更普遍的说法是 Snapdragon 800，它出现在 Nexus 5 和 2013 年的许多其他旗舰设备中。eMBMS 在诸如体育场之类的地方可用于向观众的设备进行广播。在移动网络上运行这项技术(这就是 eMBMS)意味着，对于发送给许多人的数据，例如新的软件更新，LTE 上的用户可能会因为这项技术而面临更少的网络拥塞。

eMBMS 是多播，但在移动数据网络上。它旨在提供紧急警报、软件更新、直播服务以及移动电视和广播。美国的威瑞森已经推出了这项服务，并且在最近几年的一些赛事中也有应用。这项技术在 2014 年 2 月由威瑞森在超级碗 XLVIII 的一次大型活动中首次展示。三星 Galaxy Note 3(第一批 Snapdragon 800 设备之一)被使用，人们可以选择的各种观点被传输到每个设备。视频以 1.8Mbps 的速率播放，数据输入速率为 750Kbps。除此之外，诺基亚记录了 eMBMS [由于其效率，实际上降低了提供商的成本](https://insight.nokia.com/embms-more-efficient-use-spectrum)。所有这些都是为了应对我们最终将面临的[1000 倍数据挑战](https://www.qualcomm.com/invention/1000x)。

* * *

## 什么是 1000 倍数据挑战？

1000 倍数据挑战是一种现象，高通正试图在它成为一个大问题之前解决它。在这种情况下，有太多的设备需要 1000 倍于给定时间所能提供的带宽。[根据思科 2017 年 6 月的一项最新研究](https://www.cisco.com/c/en/us/solutions/collateral/service-provider/visual-networking-index-vni/complete-white-paper-c11-481360.html#_Toc484531491)，预计到 2021 年，互联网上用于视频的数据量将高达 82%。这是一个巨大的带宽。为了显示我们看了多少视频，思科声称每个月我们将消耗超过 500 万年的视频。

幸运的是，有了多播和 eMBMS 技术，这个挑战可以被恰当地面对。我们可以从 eMBMS 或 LTE 广播技术形式的更高效、更长期的解决方案中受益，而不是不断提高服务器功率和成本，特别是现在它已经被纳入 AOSP 的来源。这意味着理论上，下一个版本*的任何 Android 设备都应该*支持 eMBMS，因为 800 系列以来的任何骁龙设备都支持它。目前，支持这项技术的主要领先者如下:美洲的威瑞森、亚洲的 Kt 和 Reliance 以及欧洲的 EE 和沃达丰。我们希望看到更多的网络提供商提供这种技术，因为随着现代连接的发展，在任何地方访问一个不拥挤且工作正常的互联网连接有时是至关重要的。