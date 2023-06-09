# 轻松地将 OpenDelta 功能添加到几乎任何 ROM 中，以节省带宽

> 原文：<https://www.xda-developers.com/easily-add-opendelta-functionality-to-almost-any-rom-to-save-bandwidth/>

[OmniROM](http://forum.xda-developers.com/omni) 最有趣的一个特点就是 [OpenDelta](http://www.xda-developers.com/android/skip-the-wait-and-save-your-bandwidth-omnirom-adds-incremental-ota-system/) 。这款创新的 OTA 系统由 XDA 资深知名开发者 [Chainfire](http://forum.xda-developers.com/member.php?u=631273) 创建，使用 open delta 技术以一种简单、带宽友好的方式带来更新。简而言之，OpenDelta 只下载自最后一次夜间下载以来更新过的文件。

如果你认为 OpenDelta 是 OmniROM 才有的特性，那你就对了。但这是一个开源项目，所以将其移植到其他 rom 上是完全可能的。如果你想知道如何将它添加到你的 ROM 中，XDA 资深会员 [werty100](http://forum.xda-developers.com/member.php?u=4240105) 制作了一个图片指南，完整地解释了 OpenDelta 的用法。通过 werty100 的指南，你将学习如何设置 Eclipse 来编译一个 OpenDelta APK，更重要的是，哪些值应该被改变以与其他具有 nightlies 的 rom 一起工作。

要将增量 OTA 系统完全合并到任何 ROM 中，只有两个文件需要一些 XML 更改。而且由于它不像 Java 或 Smali 那么难，几乎每个人都应该能够将它添加到他们的 ROM 中。

如果你渴望了解更多关于如何让 OpenDelta 在几乎每一个 ROM 上工作的知识，请到[原始线程](http://forum.xda-developers.com/showthread.php?t=2756775)中查找所有相关信息。