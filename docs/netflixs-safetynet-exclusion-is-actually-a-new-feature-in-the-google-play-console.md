# 网飞的安全网排除功能实际上是 Google Play 控制台中的一项新功能

> 原文：<https://www.xda-developers.com/netflixs-safetynet-exclusion-is-actually-a-new-feature-in-the-google-play-console/>

上周，关于网飞应用程序在搜索 Play Store 时对根用户隐藏的新闻在整个社区掀起了波澜。起初并不清楚为什么会发生这种情况，但网飞发表声明称这是有意为之。该公司表示，他们正在使用谷歌的 Widevine DRM 来阻止不受支持的设备，但这没有意义，因为它仍然可以很容易地被侧加载。

相反，看起来网飞正在使用某种安全网检查来确定该应用程序是否会作为搜索结果出现在 Play Store 中。现在谷歌 I/O 已经启动，该公司正在为他们的大量服务推出新功能，Google Play 控制台就是其中之一。看起来这里有一个新的特性，允许开发者根据一些额外的变量从人们那里排除他们的应用程序或游戏。

可以这样做，这样你的图形密集型游戏就不会显示给只有 1GB RAM 的人，或者可以这样应用，这样在不支持的 SoC 上的人就看不到你的工作。这里还有一个选项，可以在这里启用**安全网排除**。这意味着开发者可以隐藏他们的应用程序，不让那些没有通过安全网检查，或者没有通过基本完整性检查的设备看到，甚至不让那些没有通过谷歌认证的设备看到。

这实际上与我们大多数人习惯的传统安全网检查有点不同。使用标准检查，检查是在应用程序启动时进行的，如果测试没有通过，它会将您引导到一个错误页面。如果没有通过某些测试，这种设备目录排除功能可以防止人们在 Play Store 中看到该应用程序，这很有意思，因为该应用程序仍然可以进行侧加载(假设应用程序本身不存在 SafetyNet 检查)，并将继续正常工作。

我只能假设这将导致越来越多的人使用第三方应用程序库网站，如我们自己的 [XDA 实验室](https://www.xda-developers.com/xda-labs/)作为绕过这个问题的一种方式。

* * *

[**来源:安卓开发者博客**](https://android-developers.googleblog.com/2017/05/whats-new-in-google-play-at-io-2017.html)

[**Via:安卓警察**](http://www.androidpolice.com/2017/05/18/netflix-just-start-google-play-console-lets-developers-exclude-app-availability-devices-dont-pass-safetynet/)