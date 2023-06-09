# 华为与 Phoenix OS 的开发者合作开发了 Mate 10 的简易投影功能

> 原文：<https://www.xda-developers.com/huawei-mate-10-easy-projection-phoenix-os/>

虽然该公司在美国几乎没有业务，但华为是世界上排名前三的智能手机制造商。其子公司 Honor 的目标是以低价智能手机渗透印度市场。在其他地方，华为[最近在全球几个市场推出了](https://www.xda-developers.com/huawei-mate-10-pro-porsche-official/)华为 Mate 10 和 Mate 10 Pro，有传言称该设备也将[在美国推出](https://www.xda-developers.com/exclusive-att-huawei-mate-10-pro-firmware/)。除了该公司的[海思麒麟 970](https://www.xda-developers.com/huawei-kirin-970-soc-details-cortex-a73/) SoC 提供的人工智能功能，该公司最广为人知的功能之一是轻松投影。虽然[不如](https://www.xda-developers.com/samsung-announces-linux-on-galaxy-for-dex/)[三星 DeX](https://www.xda-developers.com/a-look-at-galaxy-s8-and-s8-software/) 强大，但它带来了类似桌面操作系统的体验，而无需购买昂贵的配件。华为正在其旗舰设备上推广这一功能，尽管媒体尚未真正提到轻松投影。在华为轻松投影功能的背后，是一个相对闻所未闻的玩家——凤凰操作系统的开发者北京卓超科技。

*华为的轻松投影功能。来源:[华为](http://consumer.huawei.com/en/phones/mate10-pro/)。*

Phoenix OS 是一个基于 Android 的操作系统，适用于 x86 芯片平台的电脑，尽管他们也为一些现有的 ARM 设备提供定制的 rom。它不像[的 android-x86](http://www.android-x86.org/) (尽管在一些公众压力下[开放了他们的内核源代码](https://www.xda-developers.com/petition-phoenix-os-open-source-kernel/))，但这是一种给旧设备注入新生命的简单易行的方法。

当华为[宣布其简易投影功能](https://www.youtube.com/watch?v=UTwV9cJ2c_M)时，该公司没有提到其与北京卓超科技有限公司的明显合作，以将凤凰操作系统引入华为 Mate 10。不过，这并不太令人惊讶，因为该公司正在寻求推广自己的产品，而不是其他产品。但当我试图在网上营销材料和华为公关中找到更多关于该功能的信息时，我什么也找不到。

然而，通过深入研究 Easy Projection 特性背后的 apk(hwpc explorer 和 HwPCSystemUI ),我找到了一些关于 Phoenix OS 的参考资料。首先，Phoenix OS 的徽标被隐藏在 APKs 资源文件夹中。但是最明显的证据是两个直接链接，直接指向 Phoenix OS 的网站。

```
 <string name="about_forum">Forum: http://bbs.phoenixstudio.org/</string>
<string name="about_official_site">Official site: http://www.phoenixstudio.org/</string> 
```

如果你进入 Phoenix OS 网站并导航到其[关于页面](http://www.phoenixos.com/about)，你会看到该公司在其时间表中列出了以下事件:

2017 年 10 月是华为 Mate 10 上市的同一个月，华为绝对可以算作“一线手机制造商”。在这份声明的正下方，华为也被列为该公司的合作伙伴之一。因此，我们相当肯定这两家公司之间的联系。

目前还不清楚凤凰操作系统的开发者北京卓超科技对华为轻松投影功能的贡献到底有多大。很明显，两家公司之间有某种形式的合作，我认为将大部分工作归属于任何一方都是不公平的，因为它肯定需要对 EMUI 进行大量修改才能如此紧密地集成。

这种功能可能不会移植到其他设备上，我们也不太可能在其他运行 EMUI 8 的华为或 Honor 设备上看到这种功能，除非这些设备通过 USB Type-C 支持 USB 3.1。Honor V10 不支持，但即将推出的华为设备[可能是华为 P11](https://www.xda-developers.com/exclusive-huawei-p11-has-iphone-x-style-notch/) 很可能会支持。

华为与凤凰操作系统开发者的合作很有趣，我很好奇它到底是如何运作的。这个实现让我想起了 Maru OS，这是一个很有前途的开源项目，但是似乎因为缺乏兴趣而失败了。三星最近宣布，他们将支持几个 GNU/Linux 发行版，如 Ubuntu 16.04 到 DeX，这比华为的 Easy Projection 功能更胜一筹。

尽管如此，我们还是很兴奋地看到公司正在继续模糊智能手机和台式机之间的界限。摩托罗拉短暂的 Atrix 智能手机是弥合这一差距的第一次尝试，令人失望，但随着华为和三星重新燃起兴趣，智能手机桌面体验有望变得更好。