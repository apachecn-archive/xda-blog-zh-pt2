# 谷歌手机现在可以安装在 Play Store 的非像素手机上

> 原文：<https://www.xda-developers.com/google-phone-non-pixel-play-store-download/>

**更新 1 (08/11/2020 @ 03:53 PM ET):** 谷歌手机应用的最新测试版似乎可以安装在大多数手机上。滚动到底部了解更多信息。下面保留了 2020 年 4 月 10 日发表的文章。

谷歌手机应用是谷歌的默认拨号应用，预装在 Pixel 智能手机、Android One 智能手机以及最近在欧洲销售的[小米智能手机](https://www.xda-developers.com/xiaomi-pre-install-google-phone-messages-global-european-phones/)上。如果不使用[修改的应用](https://forum.xda-developers.com/android/apps-games/app-google-phone-v14-0-175904292-bubble-t3708218)或 [Magisk 模块](https://github.com/Magisk-Modules-Repo/GoogleDialerFramework)，通常不可能在其他设备上安装该应用，但今天我们发现该应用的最新版本可以直接从谷歌 Play 商店安装在某些设备上。

我们第一次得到这种可能性的提示是由 [XDA 资深会员 springer.music，他说](https://forum.xda-developers.com/zenfone-6-2019/themes/official-google-phone-app-installed-root-t4080537)最新的谷歌手机应用可以安装在运行[最新 ZenUI 更新](https://www.xda-developers.com/asus-zenfone-6-asus-6z-update-volte-vowifi-more-carriers-march-2020-security-patches/)版本 WW_17.1810.2003.144 的华硕 ZenFone 6 上。在[华硕官方 ZenTalk 论坛](https://zentalk.asus.com/en/discussion/25472/google-phone-app-is-available-to-asus-6z)上的多名用户也证实了这种可能性。出于好奇，我决定试试能否在自己的一些设备上安装这款应用。你瞧，我设法跳上谷歌 Play 商店，把这个应用程序下载到我的运行 [ColorOS 7.1](https://www.xda-developers.com/coloros-7-1-review-on-oppo-find-x2/) 的 [OPPO Find X2 Pro](https://www.xda-developers.com/oppo-find-x2-pro-hands-on-first-impressions/) 上。具体来说，我安装的版本是版本 47.0.305350684-publicbeta。当我第一次安装谷歌手机应用程序时，我遇到了一个警告，电话可能无法工作，因为该设备是“不兼容的”，但在授予它各种权限并使其成为我的默认拨号应用程序后，我能够成功地拨打和接听电话。辅助拨号、来电显示&垃圾信息和附近的地方等功能似乎都可用，但像通话屏幕这样的像素特定功能却不可用。

XDA 的 Max Weinbach 也证实，他可以在他的 LG V60 ThinQ 上安装该应用程序，并拨打和接听电话，但他无法在他运行 OxygenOS 的一加 6T 或运行 One UI 2.1 的三星 Galaxy S20 Ultra 上安装该应用程序。我也无法在我的一加 7 Pro 上安装该应用程序。这可能是一个迹象，表明谷歌计划将对谷歌手机应用的支持扩展到更多设备，也可能只是谷歌偶然忘记将这一更新标记为与某些设备不兼容。

我们简要检查了清单，发现该应用程序仍然需要 com . Google . Android . dialer . support 共享库。三星 Galaxy S20 上没有这个共享库，这就是该应用程序拒绝安装在其上的原因。然而，这个库出现在 OPPO Find X2 Pro 和华硕 ZenFone 6 上，这可能解释了为什么这款应用程序可以安装在这些设备上。要检查您自己的设备上是否存在该库，您可以运行以下 ADB shell 命令:

```
 pm list libraries | grep "com.google.android.dialer.support" 
```

你可以从下面的谷歌 Play 商店链接或者从 APKMirror 下载最新版本的谷歌手机应用。让我们知道该应用程序是否适合您！

*本文更新于美国东部时间 2020 年 4 月 10 日下午 5:45，添加了更多关于为什么该应用程序现在似乎可以兼容更多设备的细节。美国东部时间下午 6:05 的另一个更新是添加所需的共享库也存在于华硕 ZenFone 6 上。*

* * *

## 更新 1:大多数手机

[*AndroidPolice*](https://www.androidpolice.com/2020/08/11/google-phone-app-beta-can-now-be-installed-from-the-play-store-on-pretty-much-any-phone/) 今天报道称，选择加入[谷歌手机应用的测试程序](https://play.google.com/apps/testing/com.google.android.dialer)将允许你在大多数非谷歌 Pixel 手机上安装该应用。该出版物能够在包括三星 Galaxy S20 Ultra、三星 Galaxy Z Flip、一加 8、一加 8 Pro、一加 7T 和一加 6T 在内的设备上成功安装测试版。Reddit 上的几个[一加手机用户也成功地在他们的设备上安装了该应用程序(h/t](https://www.reddit.com/r/oneplus/comments/i7mnki/anyone_else_able_to_install_the_google_phone_beta/) [Some_Random_Username](https://forum.xda-developers.com/member.php?u=8234677) )，有一些报道成功地[侧装了谷歌手机应用程序的版本 53.0.325742234-publicbeta](https://www.apkmirror.com/apk/google-inc/google-phone/google-phone-53-0-325742234-publicbeta-downloaded-release/) 。在 Play Store 的谷歌手机应用程序网页列表上， *AndroidPolice* 发现许多其他设备也被报道与该应用程序兼容。

关于设备兼容性的这一明显变化的一个警告是，你不会通过在谷歌 Play 商店搜索轻易找到谷歌手机应用。注册测试版后，你需要发送或点击该应用的 Play Store 列表的直接链接(如上面嵌入的链接)，以便从 Google Play 安装该应用。

虽然谷歌手机应用程序不提供所有地区的通话记录或大多数非像素设备的通话屏幕，但它提供了一流的垃圾邮件检测和反向电话号码查找。试试[注册测试版](https://play.google.com/apps/testing/com.google.android.dialer)，如果它能在你的设备上运行，请在下面的评论中告诉我们！