# 谷歌新闻测试文章的黑色主题和向上/向下投票按钮

> 原文：<https://www.xda-developers.com/google-news-dark-theme-articles-upvote-downvote-buttons-feed/>

基于你的兴趣和一些机器学习，谷歌新闻为你提供了从互联网上不同的出版物和博客中抓取的新闻文章的精选提要。您还可以订阅特定的出版商，或者只需轻按一个按钮，就可以阅读关于特定主题的更多信息。简单地说，它是普通用户可能关心的所有新闻的中心。该应用程序正在慢慢改进，增加了新功能；例如，最近这款应用获得了让你用两种语言查看新闻文章的能力。很快，该应用程序可能会增加两个新功能来改善阅读体验:文章的黑色主题和手动管理你的订阅的投票按钮。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

**WebView 中的黑暗主题**

去年，谷歌新闻[就像 Play Store 上的大多数其他谷歌应用一样，进入了黑暗模式](https://www.xda-developers.com/google-news-5-5-dark-theme/)。然而，这种黑暗模式主要局限于应用程序自己的用户界面。菜单以深色显示，一些新闻文章也是如此，只要它们是由应用程序而不是 Android 系统 WebView 原生呈现的。对于在 WebView 中打开的文章，背景颜色仍然是浅色的。如果你在晚上使用应用程序浏览新闻，那么这可能会很烦人。不过，在不久的将来，这款应用将会以深色背景打开网络视图。XDA 的米沙·拉赫曼在最新版本的新闻应用中手动激活了这项功能。

 <picture>![](img/163de915e6b3667ee4be28023d396ba3.png)</picture> 

The AMP version of our website forced dark by the Google News app.

该功能可能需要基于 Chromium 构建的 WebView 版本，这些版本具有最新的强制黑暗模式代码。不过，Chrome 中的强制黑暗模式仍然是不确定的，所以这一功能向用户推出可能需要一些时间。

**订阅源中的投票**

谷歌还计划在谷歌新闻应用程序中添加一个向上投票/向下投票功能，该功能采用拇指向上和拇指向下的形式。这将从本质上帮助你管理你的订阅，因为你可以很容易地告诉应用程序你喜欢哪些新闻来源/话题，不喜欢哪些。

谷歌新闻应用程序中的向上投票/向下投票按钮。点击大拇指会让应用程序向你显示类似的故事，而大拇指向下按钮会表明你不想看到这样的内容。

这些功能对用户来说还不可用，也不能保证它们会很快可用。然而，鉴于它们基本上是完整的，我们希望在未来版本的应用程序中，它们能够面向更广泛的公众。

* * *

*感谢 PNF 软件为我们提供了使用许可 [JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev) ，这是一款针对 Android 应用的专业级逆向工程工具。*