# 所有 Play Store 应用最终都需要获得谷歌的批准，才能在后台访问位置信息

> 原文：<https://www.xda-developers.com/android-apps-background-location-google-approval/>

Android 11 的第一个开发者预览版[即将发布](https://www.xda-developers.com/android-11-developer-preview-1-google-pixel/)，将会有大量的变化等待我们去发现和分析。鉴于它仅仅是*刚刚*出来，我们才刚刚开始发现新的功能。然而，在谷歌的 Android 开发者博客上，他们概述了一个可能对确保用户隐私有很大帮助的变化，而且它不会只为 Android 11 保留。开发者最终将需要直接获得谷歌的批准，以便他们的 Play Store 应用程序能够在后台获得位置服务。

随着 Android 10 的发布，谷歌使得[用户必须明确允许应用程序在后台访问位置服务](https://www.xda-developers.com/android-q-privacy-permission-controls/)。目前，当应用程序请求定位时，会出现一个提示，允许访问，允许使用应用程序，或完全拒绝访问。谷歌似乎更进一步，开发者现在需要直接通过该公司。在他们的博客文章中，谷歌表示，超过一半的用户选择了“当应用程序正在使用中”选项。在 Android 11 中，用户还可以选择只允许应用程序访问一次位置数据，应用程序下次启动时需要再次请求。

至于在后台访问位置数据的应用程序，谷歌发现许多应用程序“实际上并不需要它。”该公司将考虑以下因素，以决定应用程序是否需要在后台访问位置的能力。

*   该功能是否向用户传递了明确的价值？
*   用户会希望应用程序在后台访问他们的位置吗？
*   该功能对应用程序的主要目的是否重要？
*   你能在不访问后台位置的情况下提供同样的体验吗？

这些是谷歌在更新 Google Play 政策后将考虑的因素。Google Play 的信任与安全团队成员将审核所有此类许可请求。谷歌给出了以下三个应用程序示例，说明如何为运行 Android 11 的设备授予权限。

> #### 一个将发送紧急或安全警报作为其核心功能的一部分的应用程序——并清楚地向用户传达为什么需要访问——将有很强的理由请求后台位置。
> 
> #### 一个允许用户选择不断与朋友分享位置的社交网络应用程序也有很强的理由在后台访问位置。
> 
> #### 具有商店定位器功能的应用程序只需在用户可见时访问位置即可正常工作。在这种情况下，根据新政策，应用程序没有足够的理由请求后台位置。

这一政策变化不是立竿见影的，需要时间来实施。谷歌预计推出时间表如下。

*   **4 月**:Google Play 官方政策更新，带后台位置
*   **5 月**:开发者可以通过 Play 控制台请求对其用例的反馈，预计回复时间为 2 周，具体取决于数量
*   **8 月 3 日:**所有提交到 Google Play 的访问后台位置的新应用都需要获得批准
*   **11 月 2 日:**所有请求后台位置的现有应用都需要获得批准，否则将从 Google Play 中删除

谷歌目前鼓励所有开发者审查他们的应用程序，并确保当他们请求后台位置访问时，是出于正确的原因。开发人员还负责任何第三方 SDK 可能会尝试和访问位置在后台。这一变化影响的不仅仅是 Android 11，因为应用程序将从谷歌 Play 商店中完全删除。

我们已经详细介绍了 Android 11 中的所有主要新功能[，以及所有的](https://www.xda-developers.com/android-11-developer-preview-new-development-features/)[新隐私和安全改进](https://www.xda-developers.com/android-11-developer-preview-privacy-security-features-changes/)，所以一定要看看它们！

* * *

**来源:[谷歌](https://android-developers.googleblog.com/2020/02/safer-location-access.html)**