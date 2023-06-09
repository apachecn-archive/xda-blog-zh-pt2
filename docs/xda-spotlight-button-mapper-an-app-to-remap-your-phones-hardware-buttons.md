# XDA 聚焦:按钮映射器，一个重新映射手机硬件按钮的应用程序

> 原文：<https://www.xda-developers.com/xda-spotlight-button-mapper-an-app-to-remap-your-phones-hardware-buttons/>

硬件按钮在 Android 设备上越来越难找到，如今大多数设备都只保留了必要的电源和音量按钮。虽然一些用户喜欢屏幕导航按钮提供的圆滑设计，但其他人却不喜欢可以用于特定目的的触觉按钮。幸运的是，有了一个叫做**按钮映射器的应用程序，你可以两全其美。**

[在谷歌 Play 商店](https://play.google.com/store/apps/details?id=flar2.homebutton&hl=en)上可用，这个工具是由 XDA 公认的开发者 [flar2](https://forum.xda-developers.com/member.php?u=4684315) 开发的，它可以让用户重新映射硬件按钮来激活不同的功能**而无需 root** 。该应用程序通过利用 Android 内置的可访问性框架来工作，这意味着该应用程序可以与大多数设备一起工作，包括运行在 KitKat 等旧版本 Android 上的设备。

* * *

## 控制你的硬件按钮

这个应用程序有两个版本:基础版和专业版。基本版只限制拦截物理 home 和音量键*，但不限制你在这些按键上可以执行的动作。如果你以相当合理的价格升级到专业版(€欧盟居民 2.60 美元，美国居民 2.99 美元)，你将可以访问**主题**，设置**自定义振动级别**，更多硬件按钮支持(前提是你的手机有这些按钮)，以及在某些应用程序中重新映射黑名单按钮。如果你有一个物理 home 键，Pro 版本还提供了两个额外的功能- **锁屏窥视**和**主屏锁定**，我们将在下面介绍。*

当你第一次打开应用程序时，你会看到应用程序能做什么和不能做什么的说明。按钮映射器也没有隐藏它的局限性，并且明确声明它只能在屏幕打开时拦截硬件按钮(不是电源按钮)。为了做到这一点，应用程序请求您启用其可访问性服务。Flar2 非常明确地表示，他的应用程序尊重你的隐私，辅助功能服务仅用于拦截硬件按钮的按下。

我个人在我的设备上只有很少的硬件按钮——音量增大、音量减小和电源——只剩下两个按钮需要重新映射，因为电源按钮无法被拦截。这对于许多用户来说是相当典型的(尽管三星和一加设备的所有者将有更多的机会利用这个应用程序)，所以你可能会问自己:*这个应用程序仍然值得这个价格吗？*

在我看来，的确如此。我很快发现，只有两个按钮并不像乍看起来那样限制。这是因为我实际上可以为每个按钮设置 **3 个动作(单击、双击或长按)，这样我的可用硬件按钮总共有 6 个动作。公平地说，我不建议你真的覆盖默认的单次点击动作来调高和调低音量，但是如果你想的话，你完全可以这么做。**

*按钮映射器主题*

那么你能重新映射你的按钮来做什么呢？以下是受支持操作的(长)列表:

*   **应用程序**
    *   启动手机上任何已安装的应用程序
*   **快捷键**
    *   启动手机上任何可用的快捷方式
*   **动作**

    *   航行
        *   主页
        *   背部
        *   最近的应用
        *   最后一个应用程序
    *   援助
        *   搜索
        *   启动“助手”应用程序(相当于长按 home)

    *   用户界面
        *   关闭快速设置
        *   展开/关闭通知阴影
    *   显示
        *   切换手电筒
        *   调出电源对话框
        *   关闭屏幕
        *   拍摄屏幕截图
        *   亮度+/-
    *   声音的
        *   切换免打扰模式
        *   音量+/-
        *   下一首/上一首曲目
        *   播放/暂停

正如我们之前提到的，在高级选项菜单中有一些有用的设置。首先，有各种“旁路”选项。当系统对话框出现在屏幕上时、使用摄像头时、正在打电话时或使用您列入黑名单的任何应用程序时，您可以将按钮映射器设置为禁用。此外，您可以为按钮映射器识别有效输入的时间设置更短/更长的延迟。这对按下按钮组合过快或过慢的用户很有帮助。我建议你尝试计时，直到你找到一个你能 100%把握的时间。

* * *

## 给你的纽扣重新布线

我肯定能想到一些有用的理由来解释为什么我会继续使用这个应用程序。我做的第一件事是为 Spotify 和电话呼叫添加一个例外，这样我可以继续使用这些应用程序中的正常音量功能，但仍然保留我的自定义硬件映射。我设置的另一个动作是长按音量降低键来触发截屏，这对于我的大箱子来说通常更困难。接下来，我重新映射了长按音量增加键以返回到上一个活动的应用程序，还双击了我的音量键以显示最近的应用程序列表。

虽然我在这里的使用是相当基本的，但是在我乘地铁上下班的时候，它们非常好用。我一只手抓着扶手，另一只手拿着手机。对我来说，将两到三个步骤重新映射到一个键上要方便得多，因为我经常单手使用手机。长按切换到上一个活动的应用程序可能听起来有点奇怪，但我在复制文本时经常使用它。我发现一些应用程序不能很好地共享/复制文本，所以这个按钮 remap 使应用程序之间的跳跃更快，例如复制或输入双因素验证码。

不过，并不是每部手机的硬件按钮都像我的一样有限。~~例如，OnePlus 3/3T 的滑动按钮可以通过这个应用程序重新映射到您选择的操作。~~ **更新:**一加设备上的通知滑块似乎没有发送按键事件，因此无法被拦截。Xperia 手机通常有一个专用的相机按钮，也可以重新映射。三星设备有物理导航键，所有这些都可以重新映射以满足您的需求。例如，你可以切换三星设备上的 back 和 recents 键，以更好地反映 Android 导航布局。使用三星 Galaxy 设备，您还可以调整按钮灯(基础版)和振动持续时间(专业版)。

 <picture>![](img/bfe85acf0d64f57cc2f4d54ddd154617.png)</picture> 

Samsung Galaxy S6 Capacitive Buttons. (Credits: *[AndroidExplained](https://www.androidexplained.com/galaxy-s6-disable-capacitive-buttons/)*)

如果你的手机有一个专用的物理 home 键，你可以利用我在本期聚焦开始时提到的两个功能:锁屏窥视和主屏锁定。前一个功能允许您在锁定屏幕上释放 home 键来锁定您的设备，后一个功能允许您在主屏幕上锁定您的设备(不需要 Nova 启动器)！使用锁屏窥视，您可以按住主屏幕按钮调出锁屏(并“窥视”您的通知)，然后释放主屏幕按钮关闭屏幕。主屏幕锁定更简单，但对于那些电源按钮失灵的人来说，这是一个至关重要的功能。

开发者在他的 Play Store 描述中列出了这个应用的一系列不同的潜在用途，在他的 [XDA 论坛帖子](https://forum.xda-developers.com/android/apps-games/app-button-mapper-customize-hardware-t3361340)中也列出了一些。不过，归根结底，你能做什么完全取决于你的想象力。我们的常驻 Tasker 爱好者 Mishaal Rahman 指出，虽然您可以使用 AutoInput 这样的插件来设置 Tasker 拦截按钮按压，但使用 Button Mapper 这样的专用应用程序要简单得多。此外，由于能够启动快捷方式，按钮映射器基本上允许您执行几乎任何您可以想到的操作，这意味着您可以通过单次(或两次或长时间)按压直接启动 Tasker 任务。

* * *

## 结论

在未来的版本中，最好是在使用单独的应用程序时有不同的映射，有点像每个应用程序的“概要文件”。例如，我可能想让 Spotify 通过音量调高/调低按钮来改变曲目，但在桌面上让这些按钮打开手电筒或下拉快速设置。但目前，按钮的重新映射适用于整个系统，不适用于任何单个应用程序。

不过，总的来说，这是 Android 发烧友武库中相当有用的工具。无论你是用它来以更典型的方式重新映射你的硬件按钮，比如调高或调低音量来改变音乐曲目，还是用它来以更非传统的方式使用它，比如在我的情况下，你如何使用它取决于你的个人偏好。这个应用程序可以让你随心所欲地发挥创造力，不过，你拥有的硬件按钮越多，乐趣就越多。

* * *

[**从谷歌 Play 商店下载按钮映射器！**](https://play.google.com/store/apps/details?id=flar2.homebutton)