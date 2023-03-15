# 谷歌详细介绍了“信任令牌”，它是网络浏览器第三方 cookies 的替代品

> 原文：<https://www.xda-developers.com/google-details-trust-tokens-api-alternative-third-party-cookies-web-browsers-chrome/>

早在 2020 年 1 月，谷歌就曾提到其打算在未来两年内逐步淘汰谷歌 Chrome 浏览器的第三方 cookies。像隐私沙盒这样的倡议被认为是健康的、广告支持的网络的驱动力，将使第三方 cookies 变得过时。虽然我们还远未达到这一目标，但谷歌现在展示了它提出的第三方 cookies 的替代品:信任令牌。

在互联网环境中，cookie 是当用户访问网站时存储在用户设备上的一段数据。cookie 存储与用户与网站交互相关的数据，例如添加到购物车的商品、登录数据、表单数据等等。第一方 cookies 是由被访问网站自己创建的 cookies，当您从一个页面转到另一个页面时，该网站需要它来跟踪您的活动。另一方面，第三方 cookie 是由被访问网站或用户之外的一方创建的 cookie；这些通常是指由外部内容(如广告)创建的 cookies。由于普通用户通常很少或根本无法控制提供商可以提供给他们的广告，他们无意中允许这些广告提供商基于他们在具有来自同一提供商的广告的网站上的浏览历史来跟踪和建立用户的简档。对于广告提供商来说，跟踪用户是一项重要的任务，因为这允许他们向用户提供更符合用户口味的广告，因此更有可能吸引用户的注意力和互动。虽然这个目标表面上听起来很合理，但实际上，第三方 cookies 已经被用于更邪恶的目的，践踏用户隐私而不被关注。

与 cookies 不同，信任令牌被设计为在不需要知道用户身份的情况下对用户进行身份验证。信任令牌背后的想法是区分用户和机器人，而不是跟踪每个用户。正如谷歌提到的，网络生态系统严重依赖于建立信任信号来检测欺诈或垃圾行为者，这种粗略的细分对于接收大量无效、欺诈流量的广告行业至关重要。信任令牌是非个性化的，不能用于跟踪用户，但它们是加密签名的，因此也不能被坏人伪造。

谷歌的声明没有进一步深入信任令牌的工作原理，但是如果你对进一步的细节和 T2 的实现感兴趣的话，有一个解释文档。开发人员可以通过 API 测试信任令牌。如果一切顺利，我们应该会在 Chrome 从第三方 cookies 迁移出来之前看到它们在网络上流行起来。

* * *

**来源:[谷歌博客](https://blog.google/products/ads-commerce/improving-user-privacy-in-digital-advertising)，[网络。dev](https://web.dev/trust-tokens/)**

**故事 Via:[The Verge](https://www.theverge.com/2020/7/31/21349538/google-changes-ads-data-cookies-privacy)**