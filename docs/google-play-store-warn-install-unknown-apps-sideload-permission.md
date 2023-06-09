# 谷歌 Play 商店准备隐姓埋名模式，并对可以安装未知应用的应用发出警告

> 原文：<https://www.xda-developers.com/google-play-store-warn-install-unknown-apps-sideload-permission/>

谷歌 Play 商店是你设备上最重要的应用之一(假设你运行的是谷歌的安卓系统)，或许仅次于 Google Play 服务。Play Store 是大多数开发者发布应用程序的主要方式，也是普通用户发现和维护应用程序的主要方式。但主要并不意味着独占，开发者和用户当然都有其他媒介来分发和下载新应用。然而，这些媒介可能[给最终用户](https://www.xda-developers.com/fortnite-installer-abuse-silently-install-galaxy/)带来潜在的安全风险。谷歌现在正准备让 Play Store 警告你可能安装未知应用的应用，以便让用户了解情况，并测试匿名模式设置。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

* * *

## 隐名模式

谷歌重新关注隐私，让用户重新掌控自己的数据。[更多](https://www.xda-developers.com/google-maps-google-search-incognito-mode/)和[更多](https://www.xda-developers.com/youtube-incognito-mode-hide-history-android/) Google apps 正在接收一个匿名模式选项，允许用户选择不收集他们的数据。

[谷歌 Play 商店 v17.0.11](https://www.apkmirror.com/apk/google-inc/google-play-store/google-play-store-17-0-11-release/) 包含新字符串，表明该应用程序将很快获得自己的匿名模式:

```
 <string name=<span >"</span>og_turn_on_incognito_mode<span >"</span>>Turn on Incognito mode</string>
<string name=<span >"</span>og_turn_off_incognito_mode<span >"</span>>Turn off Incognito mode</string> 
```

我们预计谷歌将很快宣布推出这一功能。

* * *

## 活动“安装未知应用程序”权限的警告

在 Android 9 Pie 中，谷歌取消了允许从谷歌 Play 商店以外安装应用程序的通用开关，也就是所谓的“未知应用程序”。相反，用户现在必须授予每个试图将 APK 排队等待安装的应用程序权限，如果这种 APK 不是来自 Play Store 的话。例如,《堡垒之夜》在安卓上有售，但由于财务原因,[没有通过 Play Store](https://www.xda-developers.com/download-fortnite-mobile-on-android-epic-games-website/) 销售。用户需要从 Epic Games 的网站上下载堡垒之夜安装程序，然后授予 Chrome(或他们选择的浏览器)下载 APK 安装程序的权限，以便对安装进行排队。一旦您完成了堡垒之夜安装程序的安装，安装程序建议您撤销浏览器的权限，以保持此门关闭，并防止静默误用。

谷歌 Play 商店很可能建立在这个概念上，提醒用户撤销其他应用程序的侧载权限，以防止应用程序悄悄地和恶意地滥用相同的权限。

```
 <string name="protect_app_installation_permissions_page_body_none">You have no apps that can install unknown apps</string>
<string name="protect_app_installation_permissions_page_deny_all_button">Deny all</string>
<string name="protect_app_installation_permissions_page_deny_button">Deny</string>
<string name="protect_home_review_installation_permissions_body_o_plus">Some apps on this device can install unknown apps, which could put your device and personal information at risk</string>
<string name="protect_home_review_installation_permissions_button_plural">Review apps</string>
<string name="protect_home_review_installation_permissions_button_single">Review app</string>
<string name="protect_home_review_installation_permissions_title">Review app installation permissions</string>
<string name="protect_home_turn_off_unknown_sources_body">Unknown apps could put your device at risk. To prevent this, go to Security settings and turn off installations from \"Unknown sources\".</string>
<string name="protect_home_turn_off_unknown_sources_button">Go to Security settings</string>
<string name="protect_home_turn_off_unknown_sources_title">Turn off app installations from unknown sources</string>
<string name="protect_play_notification_review_installation_permissions_body">Some apps on this device can install unknown apps, which could put your device and personal information at risk</string>
<string name="protect_play_notification_review_installation_permissions_button">Review apps</string>
<string name="protect_play_notification_review_installation_permissions_title">Review app installation permissions</string>
<string name="protect_settings_app_installation_permissions_body">Review apps that can install unknown apps</string>
<string name="protect_settings_app_installation_permissions_section_title">Permissions</string>
<string name="protect_settings_app_installation_permissions_title">App installation permissions</string> 
```

Play Store 正准备提醒用户审核授予其他应用的应用安装权限。我们不认为这是为了打击 Android 上的侧装应用。相反，这很可能是试图关闭一个潜在的攻击媒介。大多数用户授予了这种权限，并且一旦他们的目标实现了，就不会再费心撤销它，这就为潜在的误用打开了大门。希望谷歌的提醒不会给那些经常监控他们的侧装活动的人带来太大的困扰。

* * *

*感谢 PNF 软件为我们提供了使用许可 [JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev) ，这是一款针对 Android 应用的专业级逆向工程工具。*