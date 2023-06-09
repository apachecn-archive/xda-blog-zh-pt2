# 谷歌将在未来几周内移除未经批准的使用通话记录/短信权限的应用

> 原文：<https://www.xda-developers.com/google-remove-unapproved-apps-use-call-log-sms-permissions/>

# 谷歌将在未来几周内移除未经批准的使用通话记录/短信权限的应用

谷歌 hasa 宣布，他们将在未来几周内移除仍在使用通话记录/短信权限的未经批准的应用。

确保个人数据的安全对 Android 的成功至关重要。如果该平台因向其他应用程序泄露敏感数据而获得声誉，那么它将使人们对获得 Android 手机感到谨慎。这是许可系统的要点，谷歌多年来一直将其改进为我们今天拥有的粒度选项。去年年底，谷歌宣布他们将[限制 Play Store 上的哪些应用程序可以访问通话记录和短信权限](https://www.xda-developers.com/google-play-developer-policy-call-log-sms/)。这些是某些应用程序工作方式的组成部分，谷歌决定不给用户拒绝或允许访问的选择。

当时，该公司表示，他们给开发者 90 天的时间来更新他们的应用程序，否则他们将因违反新政策而被从 Play Store 中删除。这一变化是独一无二的，因为即使是被允许保留的应用程序，也只有在被设置为 Android 的“默认应用程序”之一时，才能访问这些数据。由于这项新政策将只允许电话和短信的默认处理程序访问这些数据(除了少数例外)，它将许多使用这些权限来实现其功能的杂项应用程序置于砧板上。这包括 Cerberus、ACR 通话记录器和 Tasker 等应用程序。

令人欣慰的是， [Tasker 能够成功地对新政策](https://www.xda-developers.com/google-restriction-sms-call-log-permissions/)的变化提出上诉，因为该政策已更新为豁免自动化应用程序，但对于使用这种类型数据的其他应用程序来说，情况并非如此。例如，Cerberus 有一个功能，允许“短信命令，以恢复丢失/被盗的电话，没有连接到互联网。”ACR Call Recorder 等电话录音应用程序使用通话记录权限，以便知道哪个电话号码要附加到哪个录音中。然而，随着这一新的政策变化，这些功能将不再可能，因为应用程序将不被允许访问呼叫日志或短信权限。

本周，谷歌就此事发表了一篇新文章，提醒可能受到这一变化影响的开发人员。这篇文章提醒他们，该公司将在未来几周内开始删除没有更新功能(或成功上诉)的应用程序。受此变更影响的开发人员将有以下两种选择:

*   提交没有这些权限的新版本。
*   提交保留权限的新版本应用程序。这样做将要求您在 Play 控制台(即将推出)中完成一份权限声明表，并将给您延期到 3 月 9 日，以删除权限或获得您的使用案例的批准。

* * *

[**来源:安卓开发者博客**](https://android-developers.googleblog.com/2019/01/reminder-smscall-log-policy-changes.html)