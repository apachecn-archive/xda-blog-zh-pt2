# 用 Xposed 改变你的状态栏透明样式

> 原文：<https://www.xda-developers.com/status-bar-transparency-xposed/>

# 用 Xposed 改变你的状态栏透明样式

使用状态栏透明样式 x 暴露模块更改透明状态栏的外观。

Android 状态栏只有黑色，没有任何透明度的时代早已被遗忘。随着 KitKat 的发布，谷歌正式在默认的启动器和系统 UI 中添加了对半透明状态和导航栏的支持，因此现在每个应用程序都可以使用透明。

Android 开发在进化，现在大部分事情都可以在 smali 中不用改一行代码就能实现。由 XDA 资深公认开发者开发的 x posed Framework[rovo 89](http://forum.xda-developers.com/member.php?u=4419114)对于用户和开发者来说都是一个强大的工具。XDA 论坛成员 [Woalk](http://forum.xda-developers.com/member.php?u=5510242) 展示的一个模块让用户能够轻松改变状态栏的透明样式。

该模块有八种可供应用的样式。该列表包括 Android L 和 HTC Sense 5 的风格，所以如果你使用的是股票 KitKat 风格，也许是时候看看它在其他发行版上的样子了。唯一的要求(除了根和安装了 Xposed)是你的 ROM 必须是 AOSP 或者接近它。将来，支持的样式列表将会扩展。

如果你想学习如何改变你的状态栏和导航条的样式，去看看[状态栏透明度模块线程](http://forum.xda-developers.com/xposed/modules/mod-translucent-style-t2811435)。从那里，只需下载、安装并启用该模块。