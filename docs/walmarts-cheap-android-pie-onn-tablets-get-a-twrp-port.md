# 沃尔玛的廉价安卓平板电脑在 TWRP 上市

> 原文：<https://www.xda-developers.com/walmarts-cheap-android-pie-onn-tablets-get-a-twrp-port/>

回到 5 月份，[沃尔玛推出了两款超实惠的](https://www.xda-developers.com/walmart-android-pie-tablets/)(好吧，姑且说“便宜”)安卓平板电脑。如果你不记得这个公告，你可能不是唯一一个。Onn 平板电脑非常简单，但它们配有键盘盖附件，运行相当干净的 Android 9 Pie 版本。此外，起价仅为 64 美元，对于廉价平板电脑来说，它们是一个不错的非亚马逊 Fire 选择。现在，感谢我们论坛上的一些开发者，你可以在 Onn 平板电脑上获得 TWRP。

然而，这并不是典型的“TWRP 移植到空白设备”的故事。在几乎所有的设备上，TWRP 需要一个解锁的引导程序来安装。缺少一个可解锁的引导加载程序是阻碍设备负载深入修改和定制的原因。没有解锁的引导加载程序，你不能闪存 TWRP，这意味着你不能走定制 rom 的道路，等等。在沃尔玛 Onn 平板电脑上启动 TWRP 的有趣之处在于，你不需要解锁的引导程序。

**[沃尔玛 Onn 平板 XDA 论坛](https://forum.xda-developers.com/walmart-onn-tablets)**

正如该端口的开发人员所写的:“这个 TWRP 版本不需要解锁引导加载程序或禁用 VBMeta 验证。”这是非常罕见的，这意味着平板电脑开箱后非常不安全。通常，锁定的引导程序意味着您不能引导未签名的引导映像或由 OEM 以外的任何人签名的引导映像。VBMeta 是包含经过验证的启动密钥的分区；它验证受保护分区(如系统和供应商)的完整性。本质上，门是锁着的，但你可以推开它。

显然，对于极其廉价的 Android 设备来说，这种完全缺乏基本安全性的情况并不罕见。据 XDA 知名开发人员 [deadman96385](https://forum.xda-developers.com/member.php?u=4222965) 称，“通常在这些廉价设备上，引导加载程序并没有完全实现，所以它会报告系统需要的一切，但它是静态的，永远不会改变，所以如果你可以通过 SP 闪存工具闪存分区，而无需快速启动，那么你就成功了。”尽管存在明显的安全漏洞，但我们不确定为什么这些设备能够通过 CTS 并获得谷歌认证，但这显然是一个应该修复的疏忽。

在任何情况下，即使您可以在不解锁引导程序的情况下启动并运行 TWRP，开发者也建议您不要这样做。更安全的做法是解锁引导程序，这样你就不会因为闪错了东西而把自己锁在设备外面。如上所述，沃尔玛 Onn 平板电脑已经运行了非常干净的、接近库存的 Android 9 Pie 版本，但有些人已经能够安装定制的通用系统映像(GSI)。如果你正在寻找一个便宜的设备，这可能是票。

**[在沃尔玛 Onn 平板电脑上了解更多关于 TWRP 的信息](https://forum.xda-developers.com/walmart-onn-tablets/walmart-onn-tablets-general/recovery-twrp-onn-android-tablets-t3999621)**