# 用 Xposed 禁用 APK 安装屏幕

> 原文：<https://www.xda-developers.com/disable-apk-installation-screen-xposed/>

# 用 Xposed 禁用 APK 安装屏幕

从 SD 卡安装 APK 应用程序时，不要浪费额外的时间。使用 AutoInstaller Xposed 模块加快安装速度。

XDA 有许多谷歌 Play 商店没有的应用程序。他们的缺席通常有几个原因:开发者账户需要钱，他们太“黑客”了，在 Play Store 上不被接受，或者只是开发者不想在最大的 Android 应用商店发布他们的作品。你可以在我们这里的各种论坛中找到很多这样的应用。

与其他一些操作系统不同，Android 允许用户直接从内部存储器安装应用程序。初始化安装时，会出现一个屏幕，显示应用程序使用的每个权限和其他重要信息。通常，您应该充分了解每个应用程序使用的所有权限。然而，如果你在格式化后一起安装 apk*和*，并且你已经从以前的经验中知道它们是安全的，安装前重复的窗口会变得有点麻烦。XDA 资深成员 [hamzahrmalik](http://forum.xda-developers.com/member.php?u=5290145) 意识到了这一点，并创建了一个 Xposed 框架模块，让你禁用这种耗时的屏幕。

在使用本模块之前，您必须记住，这些屏幕是有原因的，因此您需要明智地使用它。有些应用程序包含可能对您的设备有害或窃取宝贵信息的恶意代码，因此我们只建议在与上述情况类似的情况下使用它，并且只与知名开发人员开发的可信应用程序一起使用。

如果您打算直接安装许多 apk，并且您已经知道它们是安全的，那么您可能希望简化这个过程。前往[自动安装模块线程](http://forum.xda-developers.com/xposed/modules/mod-autoinstaller-confirmation-t2856366)，按照开篇帖子中提供的说明，享受快速和自动的应用程序安装。一旦完成，不要忘记禁用该模块，这样你就不会无意中安装恶意应用程序。