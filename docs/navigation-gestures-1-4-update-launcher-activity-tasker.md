# 导航手势随着活动启动、Tasker 插件、性能改进等而更新

> 原文：<https://www.xda-developers.com/navigation-gestures-1-4-update-launcher-activity-tasker/>

我们的导航手势应用已经推出了 6 个多月了。自从发布以来，我们已经用[新的和方便的功能](https://www.xda-developers.com/navigation-gestures-update-app-launch-android-p/)更新了应用程序几次。距离我们的[上一次大更新](https://www.xda-developers.com/navigation-gestures-oneplus-6-oneplus-5t-gestures/)已经有一段时间了，但是 1.4 版本终于来了。这次更新包括几个新的切换，启动活动，Tasker 插件，改进的沉浸式/全屏检测，以及常见的修复。

如果你不熟悉导航手势，这是一个最初设计用来隐藏导航条和添加 iPhone X 风格手势的应用程序。自发布以来，它已经获得了大量的新功能。你不必使用 iPhone X 风格的手势。你可以使用一加风格的手势，也可以随心所欲地定制。如果你不喜欢 Android 馅饼手势或者你想要更多的屏幕空间，这是一个必备的应用程序。

对所有购买了高级版的支持者大声喊出来。您的支持有助于我们继续开发该应用。此次更新增加了一些专门针对高级用户的新功能，我们将继续致力于为高级用户带来更多价值。

更新后，如果您遇到任何问题，我们建议您重新启动。有时候更新一个 app 会让 OEM 皮肤干掉辅助功能服务……或者可能会发生其他怪异的事情。重启会让它恢复原样。

## 导航手势 1.4 版变更日志

**手势**

*   增加了“**投放活动**”动作(溢价)。这让你可以直接进入你最喜欢的应用程序的某些部分。

*   增加了 **Tasker 集成** (premium)。这不仅可以让你打开和关闭药丸或导航条，而且你还可以设置一个手势来触发 Tasker 事件——这意味着你可以对手势进行编程，基本上用 Tasker 的力量做任何你想做的事情！

**行为**

*   **通过减少辅助功能服务的轮询来提高性能**。
*   **提高了电池的使用率**。
*   默认情况下，当用户锁定设备时，应用程序将不再显示导航栏。这意味着在解锁设备后的几秒钟内，你不会看到导航栏弹出。不过，锁屏快捷键会被切断，所以如果你想使用它们，你需要手动启用这个行为。
*   为 180°旋转固定增加单独的选项(从 270°选项)。
*   基本药丸位置从显示器的顶部而不是底部(改善全屏应用程序和游戏的检测)。
*   将最大自动隐藏时间从 3 秒增加到 10 秒
*   增加默认分割药丸高度
*   改进键盘检测
*   增加了备用 home 动作切换(只有运行基于 Android 9 Pie 的 OxygenOS 9 的一加设备才需要。)

* * *

## 导航手势的常见问题和功能要求

请展开下面的按钮，查看我们对常见问题列表的回答。

### 导航手势常见问题

*   救命，我卸载了应用程序，再也无法访问我的导航栏了！
    *   请连接到您的计算机并运行以下 ADB 命令:`adb shell wm overscan reset`
*   求助，我卸载了 app，原来的导航栏一直在隐藏自己！
    *   请连接到您的计算机并运行以下命令:`adb shell settings delete global policy_control`
*   我们能不能添加一个特性，让药丸在它自己的独立区域，这样它就不会和某些 UI 元素重叠了？
    *   不抱歉。我们已经将屏幕内容向下推以隐藏导航条。添加这个特性也需要我们将屏幕内容向上推。我们不能两者兼得。
*   屏幕下方有一条“白线”！
    *   这不是 bug。这是我们在 1.0.0 版本后有意做出的一项改变的副作用，因为如果没有它，许多三星、摩托罗拉和小米设备都会报告*重大错误*(例如，解锁后黑屏，导致手机无法使用。)之所以出现“白线”是因为导航栏被隐藏了 99.99%而不是 100%(即。除了一个像素，我们隐藏了整个导航栏。)所以“白线”实际上只是你的白色导航栏。我们添加了一个名为“使用全过扫描”的实验设置，它消除了白线。使用时风险自担。
*   药丸不配合三星 DeX/三星好锁！
    *   Android 阻止第三方应用程序在系统用户界面应用程序(如状态栏和锁屏)上显示覆盖图。可以使用行为设置中的黑名单功能，让原来的导航条显示在这些应用中。
*   当你从锁屏打开相机，从锁屏接听电话，或从锁屏打开快速回复的通知时，Pill 不会显示！
    *   Android 阻止第三方应用程序在系统用户界面应用程序(如状态栏和锁屏)上显示覆盖图。这也包括从锁定屏幕接听的电话、应用程序或通知。只有解锁设备后，药丸才能显示。
*   Pill 不显示在 Facebook Messenger、Drupe 或其他浮动应用中！
    *   转到实验设置，并选择“保留药丸显示在其他覆盖应用程序中。”挑信使，德鲁伊等。在这个列表中。
*   Pill 不支持屏幕锁定。
    *   我们没有办法在没有 root 的情况下模拟长按后退键。我们正在研究的一个试验性解决方案是检测手机何时进入锁定屏幕状态，并禁用 pill 以恢复股票导航条。
*   Home action 在 OnePlus 5 上不起作用！
    *   如果您启用了软件导航栏并禁用了按钮设置中的“总是启用主屏幕按钮”选项，OxygenOS 会阻止应用程序执行主屏幕操作。要解决这个问题，请**启用**的“总是启用主页按钮”选项。
*   药丸随着导航条不停的上下“跳跃”！
    *   这意味着您要么手动启用沉浸式模式(即不是从应用程序)或另一个应用程序触发了干扰我们应用程序的沉浸式模式。以下是一些可能的原因和解决方案:
        *   **Nova Launcher** :在“Look & Feel”下的“通知栏”部分，可能会有一个“隐藏导航栏”选项。如果有，请检查以确保它已被禁用。
        *   **LG G6/LG v 20/LG v 30/LG G7 ThinQ**:进入设置>显示> Home touch 按钮>隐藏 Home touch 按钮，禁用顶部的“锁定/隐藏图标”选项，取消选中列表中的每个应用。
        *   **三星 Galaxy S8/三星 Galaxy Note 8/三星 Galaxy S9** :进入设置>显示>导航条>显示和隐藏按钮，关闭 toggle up top，取消选中列表中的每个应用。

* * *

## 加入我们的导航手势测试组

在推向谷歌 Play 商店之前，我们自己测试每一个版本，但是我们在 Telegram 上也有一个测试组，你可以[加入这里来获得最新的特性](https://t.me/joinchat/GobKO0bC5BerFC9Avo-HvQ)。

* * *

## 导航手势的反馈和支持

反馈对我们来说非常重要。虽然我们有幸接触到一个拥有来自几家不同设备制造商的各种设备的大型团队，但我们很难确保每台设备都没有错误。如果您在使用我们的应用程序时遇到问题，请不要犹豫[给我们发电子邮件](mailto:navigationgestures@xda-developers.com)或在[官方 XDA 支持线程](https://forum.xda-developers.com/android/apps-games/official-xda-navigation-gestures-iphone-t3792361)中发帖。

我们计划在未来的版本中添加更多的动作，让用户有更多的选择来控制他们的设备。我们希望提供一种可以完全取代你设备上的导航条的体验。如果您认为我们应该添加一两个功能来实现这一点，请告诉我们您的想法！