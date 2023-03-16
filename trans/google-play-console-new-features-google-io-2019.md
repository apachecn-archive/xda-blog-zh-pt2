# Google Play 控制台正在获得有条件交付、内部应用共享、新指标等等

> 原文：<https://www.xda-developers.com/google-play-console-new-features-google-io-2019/>

谷歌的 Play Store 是任何安卓设备的关键组成部分。这是迄今为止在你的设备上安装 Android 应用程序最简单、最安全的方式，也是大多数 Android 体验的入口。Google Play 控制台是开发者上传应用程序版本供谷歌审查的地方，然后才发布给公众。确保这一过程尽可能快速简单，符合谷歌的最大利益。越简单，开发者就越有可能选择 Android 作为他们应用的平台。此外，开发者越容易向他们的应用推送关键更新等，用户体验就越好。用户体验越好，Play Store 获得的用户越多，谷歌受益越多。

为此，谷歌已经暗示了许多新功能来为开发者提供 Play 控制台。当开发者登录 Play 控制台时，出现了一个通知，告知开发者 Play Store 将[改变其处理评论的方式](https://www.xda-developers.com/google-play-store-app-rating-recent-reviews/)。最重要的是，上个月的这个时候，我们注意到 Play Store 的开发者设置中隐藏了一个名为[“内部应用共享”](https://www.xda-developers.com/google-play-store-developer-setting-enable-internal-app-sharing/)的新选项。当时，我们无法区分内部应用程序共享和已经众所周知的内部测试渠道之间的区别，但这是未来发展的迹象。

谷歌对 Play Store 更精简体验的追求仍在继续，3 月份他们宣布了一个更标准化的版本[应用图标](https://www.xda-developers.com/googles-new-requirements-will-make-every-play-store-icon-a-squircle/)。在此之前，去年 10 月发布了对应用捆绑包、即时应用和应用管理工具的改进。这些变化是为了减少 APK 的大小——平均减少 35%——以及通过允许用户更好地管理订阅和在下载整个应用程序之前尝试迷你版本的应用程序，使应用程序对用户更具吸引力。

很容易看出，谷歌正在积极努力，让 Play Store 和 Play Console 成为一个对所有人都更好的地方。当 Play Store 还是一个相对较新的应用程序市场时，它以不安全和通常充满垃圾而闻名。当放在苹果的应用程序商店旁边时，它的质量与应用程序商店严格管理但仍然丰富的应用程序选择相比相形见绌。如今，它要安全得多，在某些方面甚至超过了 App Store。但是谷歌离 Play Store 还远着呢。本周的 I/O 带来了大量关于谷歌的新闻。这反过来意味着我们可以听到更多关于谷歌 Play 控制台的计划。Google Play 总监 Purnima Kochikar 对一群开发人员开放了我们在未来几个月可以从 Play Store 看到的东西。

## 动态交付功能

基于去年推出的 Android 应用捆绑发布格式，谷歌正在发布向用户提供更新的新方法。Android 应用捆绑包是一种旨在减少安装大小的格式，现在是 Play Store 上发布应用的官方格式。谷歌报告称，使用这种新格式的应用程序平均节省了 20%的大小，这种大小节省的直接结果是高达 11%的安装提升。

谷歌现在正在扩展 Android 应用捆绑包，增加动态功能，改变向用户提供更新的方式。

*   按需交付-在需要时或在后台安装功能，而不是在安装时交付，并减少应用程序的大小。
*   有条件交付-根据用户的国家/地区、设备功能或最低 SDK 版本，控制在安装时交付应用的哪些部分。
*   即时体验-现在完全支持，因此您只需为您安装的应用程序和 Google Play 即时体验上传一个工件。

这对开发者意味着什么？首先:按需交付。本质上，对于更多的小众功能，开发者可以这样做，只有试图访问该特定功能的用户才会将它下载到他们的设备上。以网飞为例。网飞现在将其客户支持功能作为动态功能提供给访问支持中心的用户。通俗地说；如果任何人使用网飞应用程序试图访问网飞的客户支持，他们会将该功能下载到他们的设备上，允许他们使用应用程序内的客户支持。从不尝试联系客户支持的用户将永远不会安装该功能，从而导致应用程序大小减少 33%。

有条件交付允许开发者决定当用户点击安装按钮时下载应用程序的哪些部分。这意味着，如果一个应用程序有赌博元素，例如，如果用户生活在对赌博有严格限制的国家，开发者可能会选择不安装该应用程序的元素。开发者还可以根据设备功能限制应用元素，例如，如果设备没有 NFC，那么该应用中与 NFC 相关的功能可以从下载中删除。这让开发者能够更好地控制用户对应用的体验，并有可能减少下载量。

Instant experiences 与 Play Store 上的“立即尝试”功能相关，允许用户在下载完整版本之前尝试该应用程序的迷你游戏版本。开发者不再需要为这个特性上传一个单独的文件。他们现在可以简单地将应用程序的主要构件打包，从而实现更简化的体验。

## 内部应用程序共享

我们在文章的前面提到了内部应用共享，这是我们一个月前注意到的，但当时似乎并没有给 Play Store 增加任何东西。现在谷歌已经透露了内部应用共享的目的。核心思想是，你将你的应用捆绑包上传到 Google Play 控制台，并立即获得一个下载链接，与你的测试人员分享。这绕过了获取版本代码、签名密钥等繁琐的工作。

此外，谷歌还通过推出新安装的应用签名密钥升级来提高安全性。此次升级增加了开发者为 Google Play 新安装的签名密钥的加密强度。这消除了潜在的安全缺陷，许多开发人员用很久以前生成的密钥签署他们的应用程序。当然，这是选择加入。

## 更轻松的更新

更新是现代软件无所不在的一部分，也是最容易让用户烦恼的部分。谷歌新的应用内更新 API 允许两种类型的更新通知。“即时”流量迫使用户在允许他们继续使用之前更新应用程序。“灵活”流允许用户拒绝更新，但也允许他们在后台下载更新，同时仍然使用应用程序。在测试中，大约 50%的用户接受了更新，这大概比以前的百分比有所提高。

## 新的 Google Play 控制台数据

Play 控制台充满了旨在帮助开发人员改进他们的应用程序、找出他们的核心用户人口统计数据等的数据。现在，它正在大修。

*   **核心指标更新** —更好地了解您的获取和流失情况，包括关于回头客的数据、自动变更分析、安装方法(例如预安装和点对点共享)、指标基准测试，以及从几小时到几个季度的聚合和重复数据删除能力。
*   **应用程序大小指标和报告** —深入了解您在 Android 生命周期中的应用程序大小，包括下载大小、设备上的大小(安装时)、与同行相比随时间的变化，以及量身定制的优化建议。
*   **开发人员选择的同行基准** —创建一个由 8-12 名同行组成的定制组，与您的应用进行比较，然后查看该组的中值，以及您的应用与其他同行在 Android 生命数据以及评分等公共指标方面的差异。
*   **利用精选 peerset 进行市场洞察** —在接下来的几个月中，您还可以将您的增长与自动生成的精选 peerset 进行比较，精选 peerset 包含大约 100 个与您相似的应用，用于衡量转化率和卸载率等业务敏感指标。

更多的数据是更好的数据，很高兴看到谷歌优化 Play 控制台，尽最大努力帮助开发者。这里的大多数元素都是不言自明的，所以我们将继续。

## 用户评论

在文章的前面，我们谈到了谷歌如何改变应用程序的评级，以更加关注最近的评论。此举很有道理；如果开发人员目前高度完善的应用程序曾经是一个漏洞百出的烂摊子，他们不应该受苦。应用程序会随着时间的推移而变化，谷歌正在努力确保应用程序评论显示这一点。谷歌 Play 商店评分现在更倾向于最近的评论，更公平地反映了该应用程序的现状。

与 Gmail 中的建议回复类似，谷歌现在正在为应用评论生成建议回复。当查看评论时，开发人员会看到三个基于评论内容的自动生成的响应。目前，这些回复只有英语版本，但更多语言版本即将推出。

## 自定义商店列表

在 3 月份的 GDC 上，谷歌推出了按国家定制的列表，这意味着英国用户可能会看到与美国用户完全不同的应用页面。可以使用不同的图像以及不同风格的文本。在此基础上，谷歌现在将允许开发者根据安装状态创建自定义列表。这意味着安装了该应用程序的用户可能会看到与未安装的用户不同的页面。类似地，有应用但卸载了的用户可以看到不同的页面。这背后的想法是针对特定类型的客户，以增加他们安装/重新安装应用程序的可能性。

## 结论

上述所有特征本身都是令人兴奋的前景。但合在一起，它们最终表明谷歌对 Play Store 和 Play Console 有着宏大的计划。该公司清楚地认识到，开发者是将用户引入平台的关键，因此为他们配备了尽可能多的工具，以确保他们做到这一点。

如果你是一名 Android 开发者，一定要注册谷歌的[预注册程序](https://support.google.com/googleplay/android-developer/answer/9084187)，该程序允许开发者在应用发布前为其建立知名度。这是 Play Store 已经人满为患的 I/O 中宣布的又一项功能。

[**来源:谷歌**](https://android-developers.googleblog.com/2019/05/whats-new-in-play.html)