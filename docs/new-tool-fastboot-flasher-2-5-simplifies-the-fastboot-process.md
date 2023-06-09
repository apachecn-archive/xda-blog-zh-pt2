# 新工具-快速启动闪光器 2.5 简化了快速启动过程

> 原文：<https://www.xda-developers.com/new-tool-fastboot-flasher-2-5-simplifies-the-fastboot-process/>

圣诞节你收到新的安卓设备了吗？大约有 370 万次激活发生在 12 月 24 日至 25 日，所以可以肯定你们中的一些人激活了。你已经使用了像 [SuperOneClick](http://www.xda-developers.com/android/superoneclick-updated-to-2-2-now-features-zergrush-exploit/) 或 [HTC Super Tool](http://www.xda-developers.com/android/htc-super-tool-the-latest-all-in-one-for-your-htc-device/) 这样的工具来引导和/或解锁你的引导程序，并允许定制 ROMs 在“轻松引导”的时代，不用说闪存也应该很容易。

XDA 用户 [slayerXcore](http://forum.xda-developers.com/member.php?u=2264272) 发布了一个脚本(仅适用于 Windows ),可以自动执行快速启动和恢复中使用的大多数命令。他专注于设计一个快速、小型且(很可能)通用的脚本来为您处理这些问题。它非常容易使用，并且在我测试过的所有 8 个设备上都有效。他的“安装说明”在下面，粗体字是我强调的，不是他的。

> 把它提取到某个地方，比如你的桌面，尽管任何地方都可以。
> 
> 当我说提取它，我的意思是使用提取所有，所以你得到我的文件结构不要移动这些文件，否则它会打破*
> 
> 运行/双击 FastbootFlasher.bat
> 
> 迎接你的将是我的自述！。txt 文件，请阅读它，因为它给你一个免责声明，说我不负责你对你的设备做的任何事情
> 
> 关闭自述文件！。文本文件（textfile）
> 
> 我希望这个工具可以帮助那些不熟悉 fastboot 的人，或者帮助那些想要更快做事方式的人。
> 
> **最后一个注意事项不要给它另一个设备或一个非文件。img 文件，无论你拖放什么文件，它都会闪烁。一旦你按下回车键，它就会闪烁曾经被拖动到脚本上的内容。也不要拖着一个无线电 img 当它要求恢复或反过来，糟糕的事情会发生，虽然他们是可以修复的使用选项 3 在最后，并重复这个过程，我不希望任何人搞砸他们的设备犯这样一个简单的错误。**

你可以在这里找到他的帖子