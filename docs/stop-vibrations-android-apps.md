# 使用 ADB 命令停止任何 Android 应用程序的振动

> 原文：<https://www.xda-developers.com/stop-vibrations-android-apps/>

在线广告继续寻找新的方式来惹恼你。在过去的几年里，一种特殊形式的在线广告一直困扰着移动设备:振动广告。利用[震动 API](https://developer.mozilla.org/en-US/docs/Web/API/Vibration_API) ，广告一直在震动你的手机[恼人地抓住你的注意力](https://forum.xda-developers.com/android/help/annoying-chrome-ads-pop-vibrate-phone-t3524971)。这个问题[已经知道很多年了](https://shkspr.mobi/blog/2014/01/malicious-use-of-the-html5-vibrate-api/)，但是谷歌解决这个问题非常缓慢。只有 Chrome 60 版本取消了振动广告，但截至目前，60 版本仅在 Chrome 的 Beta、Dev 和 Canary 频道提供。然而，实际上有一种方法可以手动停止你手机上任何安卓应用的振动——而不用把你的手机完全置于静音模式。这意味着你不必等待应用程序开发人员更新他们的应用程序，这样他们就不能振动你的手机。

* * *

## 停止任何 Android 应用程序的振动

我们正在做的方法很简单。我们要做的只是通过发送 ADB 命令来限制允许应用程序使用设备振动电机的权限。这样做，应用程序就不能振动你的手机。在我们开始之前，我们需要安装一个应用程序，这样我们就可以知道我们想要阻止手机振动的应用程序的名称。别担心，这是一个完全免费(而且很小)的应用。

1.  为你的[特定设备](https://developer.android.com/studio/run/oem-usb.html)安装 USB 驱动，可能只有在你运行 Windows 时才需要。
2.  为您的操作系统下载 [ADB 二进制文件](https://www.xda-developers.com/google-releases-separate-adb-and-fastboot-binary-downloads/)。
3.  将 ZIP 文件解压到 like Downloads 上易于访问的文件夹中。
4.  进入手机设置，找到关于手机选项。
5.  在这里找到“内部版本号”的值，点击 7 次以启用开发者模式。
6.  回到设置的主菜单，进入开发者选项。
7.  启用 USB 调试模式。
8.  将手机插入电脑，从“仅充电”模式切换到“文件传输(MTP)”模式。这并不总是必要的，但可能需要在您的设备上运行 ADB。
9.  回到 PC 并导航到之前解压 ADB 二进制文件的目录。
10.  在这个 ADB 目录中启动一个命令提示符(在 Mac/Linux 上是终端)。在 Windows 上，最快的方法是按住 Shift 键，然后右键单击。在弹出的上下文菜单中，选择“在此打开命令提示符”选项。
11.  在命令提示符或终端中，输入以下命令来验证我们是否可以连接到设备:`adb devices`
12.  这将启动 ADB 守护程序。如果这是您第一次运行 ADB，您将看到一个提示，要求您授权连接。允许它。
13.  现在从步骤 11 重新运行命令，您将在输出中看到设备的序列号。如果是这样，那么你已经准备好继续前进了。如果没有，请尝试重新安装驱动程序。
14.  通过打开应用程序检查器，转到应用程序列表，然后轻按应用程序，找到您想要限制振动手机的应用程序包。
15.  执行以下命令进入手机的外壳环境:`adb shell`
16.  然后执行此命令，限制 app 使用振动电机:`cmd appops set <package> VIBRATE ignore`
17.  您不会在提示中看到任何确认，但是只要您没有收到错误消息，它应该已经工作了。

* * *

## 说明

所以我们在这里做的是限制我们选择的应用程序的权限。该权限由应用程序在它们的`AndroidManifest.xml`文件中定义，并且在安装时自动授予应用程序。虽然您可以使用内置的权限管理器来限制应用程序的某些权限，但振动权限不在其中。

相反，我们通过使用`cmd appops`命令来限制这个权限。这是“appops”的命令行界面——Android 面向用户的权限管理系统。通过 ADB shell 访问该系统，我们可以限制比平时更多的权限。我们可以撤销的权限之一是振动权限。通过这样做，我们停止振动，因为应用程序不能再使用你的手机振动电机没有必要的许可。

谷歌不希望你能够正常限制这个权限，所以他们在设置中隐藏了它。这是因为许多应用程序出于合理的原因依赖于振动你的手机，例如某些动作的触觉反馈或通知你一些事情。谷歌保留了命令行功能，以防止应用程序振动你的手机，这样开发者就可以测试如果手机没有振动电机，他们的应用程序将如何工作。然而，没有振动电机的设备很少出现，因此该命令通常不会被使用。

尽管如此，仅仅因为这个隐藏的命令没有被开发人员使用，并不意味着我们不能很好地使用它。事实上，由于这个命令，我们可以停止任何 Android 应用程序的振动了！不需要等待谷歌更新 Chrome 稳定版或 Opera 更新 Opera Mini，你现在就可以自己停止振动广告！此外，如果你知道有什么应用程序让你头疼，让你的手机振动太多(他们不允许你关闭)，现在你也可以阻止这种情况发生。接下来，我们希望谷歌 Chrome 的[广告拦截器](https://www.xda-developers.com/google-reportedly-working-on-a-built-in-ad-blocker-for-chrome-browser/)能够拦截这类广告，尽管我们只有[几天时间来测试](https://www.xda-developers.com/ad-block-google-chrome-canary-dev/)这一新功能。