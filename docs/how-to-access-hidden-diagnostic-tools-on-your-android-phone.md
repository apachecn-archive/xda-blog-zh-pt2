# 如何访问 Android 手机上隐藏的硬件诊断工具

> 原文：<https://www.xda-developers.com/how-to-access-hidden-diagnostic-tools-on-your-android-phone/>

如果你买的是二手手机，你绝对应该做的第一件事就是彻底检查手机硬件，确保一切正常。因此，你插入 SIM 卡，前往 Play Store，从众多免费的硬件诊断测试应用程序中下载一个。但是没有必要安装任何第三方应用程序，因为在大多数 Android 智能手机中，你会发现一个隐藏的硬件诊断应用程序。

毕竟，当你把手机送到制造商那里时，技术人员需要一个工具来正确评估你手机的状态，以便集中精力整修哪些部件。这就是为什么你会注意到一些奇怪的系统 apk 预装在你的手机上，乍一看似乎是某种无法访问的膨胀软件，但如果你知道如何访问它们，它们会为你提供一套在你的手机上运行的诊断测试。

免责声明:这只是我们将要分享的一个有趣的发现，因为在现实世界中，安装一个第三方应用要比在你的手机中寻找一个隐藏的应用容易得多。

* * *

****

华为的 HwMMITest

你有华为的设备吗，比如华为 Mate 8、华为 Mate S、华为 P9，甚至是 Nexus 6P？如果是这样，那么当你导航到设置->应用程序并启用显示所有系统应用程序的选项时，你会发现一个名为 **HwMMITest 的应用程序。**这是一个预装在所有华为设备上的应用程序，通常无法从任何应用程序启动器访问。

为了访问这个秘密的诊断应用程序，你需要首先重启引导程序。如何做到这一点在各种华为设备之间有所不同，但在 Nexus 6P 上，你需要做的就是在设备关闭时按住 Vol Down + Power。然后，当您进入 bootloader 菜单时，通过使用音量键滚动选项来导航到 **Factory** 选项，然后通过按下电源按钮触发引导过程来确认选项。或者，您可以尝试通过命令提示符键入**fast boot OEM enable-HW-factory**。

一旦你重新启动到 Android，你会在你的通知栏看到两个持续的通知。一个是名为**项目菜单**的秘密菜单(我不确定其目的)，第二个是名为 **MMI 测试**的菜单，如果你当前的电池电量在 55%到 80%之间，点击它将开始设备硬件的引导测试。

app 到底测试什么？一切。这里只是一个简短的列表:

*   LCD 亮度/色彩测试/坏点测试
*   触摸屏/数字化仪测试
*   前置/后置摄像头
*   指南针/GPS/重力传感器
*   光敏感元件
*   振动马达
*   扬声器测试
*   麦克风/耳机测试
*   蓝牙/WiFi/SIM 卡测试
*   等等。

* * *

虽然上面的截图来自 Nexus 6P，但它们只是华为设备上隐藏的诊断工具的指示。在其他制造商的设备上访问诊断工具需要不同的步骤。例如，在 Moto X Pure 上，你可以直接访问该工具，而不必通过[启动其隐藏活动](https://play.google.com/store/apps/details?id=de.szalkowski.activitylauncher&hl=en)来启动 fastboot。试着找出如何在你自己的设备上使用这个工具，如果你能在下面的评论中找到它，请**告诉我们！**