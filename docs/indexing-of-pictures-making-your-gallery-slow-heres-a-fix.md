# 图片索引使您的图库运行缓慢？这里有一个解决办法...

> 原文：<https://www.xda-developers.com/indexing-of-pictures-making-your-gallery-slow-heres-a-fix/>

所以，你给自己买了一个 32 GB 的 microSD 卡，里面装满了你电脑里的所有东西(就媒体而言)。一切都很顺利，但是你不能帮助和注意到你的 10 级卡应该，或者至少感觉比它在你的画廊加载图片时快一点。有很多关于如何调整 SD 卡速度的指南，它们都会有所帮助，但是由于这个特殊的原因，手边可能有一个更简单的解决方案。通常情况下，Android 的图库应用程序会扫描你的整个设备来获取图片。这意味着，在这个过程中，它会选择图标文件夹、背景文件夹、缩略图文件夹，以及任何你不想在图库中显示的内容。例如，您可能在卡片的中心有一个文件夹，其中有当前自定义主题的图标。这些将在扫描过程中被拾取。

为了把你从这种烦恼中解救出来(还有一些其他“不想要的”图片，你可能会在你的设备中到处漂浮)，有一个非常简单的解决方法。每当您不想显示某些图片或图像文件时，您只需简单地重命名包含该媒体的文件夹，并在名称的开头加上“句点”。Android 会认为这是一个隐藏的文件夹，因此，当向您提供所请求的图片时，它不会查看它。例如，一个名为 private 的文件夹，您只需将其重命名为。私人，然后嘣！问题解决了。此外，您还可以添加一个名为。nomedia 添加到包含它的文件夹中，这样也可以解决这个问题。

试一试，看看这是否适合你。

这篇快速指南摘自 XDA 成员 [SemperAndroid](http://forum.xda-developers.com/member.php?u=3136329) 的[跟帖](http://forum.xda-developers.com/showthread.php?t=1039421)。

想在门户网站上发表什么吗？联系任何新闻记者。