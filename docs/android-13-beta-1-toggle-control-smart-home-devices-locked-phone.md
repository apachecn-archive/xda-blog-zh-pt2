# Android 13 Beta 1 增加了一个新的开关，可以在锁定的手机上实现设备控制

> 原文：<https://www.xda-developers.com/android-13-beta-1-toggle-control-smart-home-devices-locked-phone/>

# Android 13 Beta 1 引入了一个新的开关，帮助你在锁定的手机上控制智能家居设备

第一个 Android 13 测试版在锁屏设置中引入了一个新的切换，将使智能家居设备控制在锁定的手机上可用。

在 Android 13 DP2 中，谷歌引入了一个新的 API 来让用户访问一些设备控制，甚至是在锁定的手机上。谷歌关于这个新的 isAuthRequired 方法的文档显示，如果它返回“true”，相关的设备控制将在锁定的手机上可用。在第一个 Android 13 测试版中，谷歌增加了一个新的开关，可以帮助你启用或禁用这一功能。

正如你在附带的截图中看到的(via*mishal Rahman*)，Android 13 Beta 1 中的锁屏设置包括一个新的“从锁定的设备控制”切换。该开关的描述如下:*“如果设备控制应用程序允许，无需解锁手机或平板电脑即可控制外部设备。”*

启用这个新的切换将可能让您访问锁定屏幕上的一些设备控制。然而，我们目前无法确认哪些设备控制将在锁定的设备上可用，因为该功能仍然需要提供控制的应用程序的支持。谷歌尚未更新谷歌主页应用程序来支持这一功能，我们目前没有从该公司获得任何关于可能发布日期的信息。

幸运的是，Tasker 开发者 [joaomgcd](https://forum.xda-developers.com/m/joaomgcd.4805489/) 已经在自动化应用中添加了一个新的开关，允许用户创建一个自定义的设备控制，即使设备被锁定也可以使用。查看下面嵌入的视频，了解它的实际应用。

值得一提的是，该功能不会让用户选择在手机锁定时可以使用哪些设备控制。相反，应用程序开发人员将不得不选择某些设备控制是否可以在锁定的手机上使用。因此，在开发人员更新他们的应用程序以支持该功能之前，该功能将不可用。

你认为哪些设备控件可以方便地添加到锁屏中？请在下面的评论区告诉我们。