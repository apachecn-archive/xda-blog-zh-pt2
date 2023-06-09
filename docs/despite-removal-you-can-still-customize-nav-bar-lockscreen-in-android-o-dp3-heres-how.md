# 尽管移除了，你仍然可以在 Android O DP3 中自定义导航条和锁屏——以下是方法

> 原文：<https://www.xda-developers.com/despite-removal-you-can-still-customize-nav-bar-lockscreen-in-android-o-dp3-heres-how/>

Android O 开发者预览版[现在已经到了第三版](https://www.xda-developers.com/android-o-developer-preview-3-rolling-out-with-final-android-o-apis/)，这意味着最终的 API 已经准备好了，谷歌正在为即将到来的发布做准备，预计在剩余的开发者预览版中只会有一些小的错误修复。在之前的 Android O 预览版中，我们看到了对用户界面的大量改进以及一些额外的定制功能，其中一些可能正在测试中，可能不会在以后的版本中提供。

事实上，用户已经报告说，在 Android O DP3 中，[锁屏快捷方式定制](https://www.xda-developers.com/android-o-preview-adds-lockscreen-shortcut-customization/)和[导航栏定制](https://www.xda-developers.com/android-o-preview-brings-nav-bar-customization-under-system-ui-tuner/)都已经从系统 UI 调谐器中删除，这表明它们实际上不会作为面向用户的功能在 Android O 的稳定版本中发布。但这并不意味着它们仍然不可访问——事实上，自从牛轧糖[以来，导航条定制在 AOSP 一直处于休眠状态。因此，虽然这一功能并不新鲜，但谷歌通过将它放置在所有隐藏的实验性功能所在的系统 UI 调谐器中，尝试将其引入最终用户。虽然我们很幸运地收到了在第一个 Android O 开发者预览版中引入的新的导航条和锁屏功能，但我们不知道何时才能恢复这些功能。默认情况下，我们很可能不会在正式版本中看到它们，甚至可能不会在系统 UI tuner 下。](https://www.xda-developers.com/nav-bar-customization-was-hidden-in-stock-nougat-all-along-and-it-never-needed-root/)

幸运的是**仍然可以在不需要访问官方界面的情况下操作这些功能**。令人惊讶的是，仅仅是面向用户的菜单被删除了，这意味着如果你想定制你的 Android O DP3 版本，你仍然可以充分利用这些功能。很可能，我们将在下面描述的非官方方法也将在官方版本中起作用，除非谷歌从系统用户界面 APK 中完全剥离负责该功能的代码，所以请将该指南放在手边，以防您无法访问预览，但希望以后对此进行实验。如果你在牛轧糖上，根据你的只读存储器，你现在可以玩导航条定制了。

**需求**:本指南针对运行 Android O 开发者预览版 3 的用户。目前，这包括 Nexus 5X、Nexus 6P、Nexus Player、Pixel C、Google Pixel 和 Google Pixel XL。锁屏快捷方式定制在运行 Android Nougat 的这些设备上不可用，但导航栏定制可用。

* * *

## 修改导航栏-应用方法

[***原创文章***](https://www.xda-developers.com/nav-bar-customization-was-hidden-in-stock-nougat-all-along-and-it-never-needed-root/)

安装[定制导航栏调谐器](https://play.google.com/store/apps/details?id=xyz.paphonb.systemuituner)和[注册 beta 测试](https://play.google.com/apps/testing/xyz.paphonb.systemuituner)以获得所有最新功能。打开应用程序，按照屏幕上的说明进行设置，它将请求 WRITE_SECURE_SETTINGS 权限，并解释授予权限的两种方式。

除非你的手机是根用户，否则你需要通过一个 ADB shell 来授予这个权限。为了做到这一点，你需要[为你的特定操作系统下载 ADB 二进制文件](https://www.xda-developers.com/google-releases-separate-adb-and-fastboot-binary-downloads/)，如果你使用的是 Windows 系统，还需要[谷歌 USB 驱动程序](https://developer.android.com/studio/run/win-usb.html)。接下来，进入设置- >关于手机，点击 7 次内部版本号，启用开发者选项。然后在设置中打开开发者选项(它会提示你输入手机的 pin/密码)并启用 USB 调试。将你的手机插入你的电脑，打开你保存 ADB 二进制文件的命令提示符/终端，然后输入`adb devices`。你的手机将提示启用 ADB 访问-授予它，然后你会看到你的手机在命令提示符/终端的序列号。

现在，您可以输入命令来授予自定义导航栏应用程序中提到的所需权限。授予应用程序此权限后，您将通过兼容性测试，应用程序将尝试修改您的导航栏。如果成功，您将能够继续并访问主菜单。

### 重新排列导航栏按钮

使用该应用程序重新排列导航栏非常容易。如上所述，确保您是一名 beta 测试人员，以便利用实验功能。你会找到一个名为**实验调整**的部分，访问它来查看允许你替换三个现有键的选项。你可以改变他们的顺序或改变他们的任何你想要的，该应用程序是非常直观的，你应该没有问题达到一个你舒服的设置。

### 自定义导航栏的其他用途

自定义导航栏应用程序有一大堆功能要浏览，所以自己去探索它的产品吧！这里是我以前写的两个教程，展示了如何在有用的情况下使用应用程序的 Tasker 集成(专业功能)。

由于该应用程序提供了触发 Tasker 事件的能力，你可以从技术上编程导航条键来执行几乎任何可以想象的动作，在任何你想要的情况下。

* * *

## 使用 ADB 进行锁屏定制

幸运的是，这个特性非常简单，因为除了添加一个快捷方式之外，没有太多的定制。锁屏快捷方式非常有用，谷歌在系统 UI tuner 中的方法非常强大——它不仅允许你选择应用程序快捷方式，还允许你选择各种应用程序的特定活动，所有这些都在一个直观的菜单中与图标一起列出。虽然这种方法不太直观和容易使用，但它仍然非常简单，你仍然可以使用 ADB 为任何应用活动添加快捷方式。您只需使用以下 synax 传递 adb shell 命令:

对于左键:

`settings put secure sysui_keyguard_left "COMPONENT/NAME"`

对于正确的密钥:

`settings put secure sysui_keyguard_right "COMPONENT/NAME"`

其中`COMPONENT`是指应用程序的包名，而`NAME`是指所述包内的活动名。例如，如果我想在左侧启动 Hangouts 的主活动，我可以输入:

`settings put secure sysui_keyguard_left "com.google.android.talk/com.google.android.apps.hangouts.phone.BabelHomeActivity"`

最后，如果您想要自定义左或右锁屏快捷键是否也自动绕过锁屏，您可以输入以下命令:

`settings put secure sysui_keyguard_left_unlock 0/1`

设置将安全 sysui_keyguard_right_unlock 0/1

其中 0 表示快捷键不会解锁手机，1 表示快捷键会解锁手机。

剩下的唯一问题是，我究竟如何确定我想要包的什么特定活动，以及我必须在命令中输入的这种活动的名称是什么？幸运的是，借助任何 [activity launcher 应用程序](https://play.google.com/store/apps/details?id=de.szalkowski.activitylauncher&hl=en)，或者您可能正在设备上使用的流行 Nova Launcher 中的 activity launcher 小部件，可以非常直观地收集这些信息。只需找到你想要的应用程序并浏览它的活动，你就有可能找到你想要的特定屏幕。

* * *

## 无穷尽

很遗憾看到可访问的、面向用户的定制这些功能的界面从最新的开发者预览版中消失，因为这标志着它们在 Android 8.0 正式版中的潜在消亡。然而，正如你所看到的，即使没有系统 UI 调谐器中的 GUI，仍然可以访问底层功能，这意味着一旦 O 出现，你将有希望继续调整导航栏和锁屏快捷方式。不要让这本有限的指南低估了这些功能:**的可能性是无限的**，因为你不仅可以在锁屏上添加任何活动的快捷方式，而且通过使用键码，你可以添加各种功能，如[媒体控制](https://www.xda-developers.com/how-to-add-media-playback-controls-to-the-nav-bar-when-playing-music/)、[浏览电子邮件](https://www.xda-developers.com/add-forward-backward-keys-to-android-o-nav-bar-quickly-read-emails/)、[滚动页面](https://www.xda-developers.com/how-to-add-page-scroll-keys-to-the-navigation-bar-while-using-chrome-in-android-o/)等等。如果你是我之前的 [Tasker 教程](https://www.xda-developers.com/tag/tasker-tutorial/)的粉丝，那么你会发现大量的方法来利用这些功能并充分利用你的设备。

* * *

你对这些特性及其去除有什么看法？有什么问题吗？留下评论。