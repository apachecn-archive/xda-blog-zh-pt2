# Android Pay 不再支持无系统 Root

> 原文：<https://www.xda-developers.com/android-pay-no-longer-working-with-systemless-root/>

轻拍。付钱。完成了。如果你拥有一部运行 4.4+的支持 NFC 的 Android 手机，那么你可能听说过 [Android Pay](http://officialandroid.blogspot.com/2015/09/tap-pay-done.html) 。该应用程序支持添加来自许多不同银行的卡，并在许多主要零售商中工作，而且它的设置也非常容易。谷歌几乎是 *[乞求](https://www.android.com/pay/tap-10-rewards/terms-and-conditions/)* 你来报名！

也就是说，除非你是一个拥有根设备的超级用户。对我们来说，我们必须在 root 访问和它带来的所有好处(广告拦截、主题化、暴露等)之间做出选择。)和使用 Android Pay。谷歌表示，限制根用户使用 Android Pay 是一项预防措施，以防止任何金融安全漏洞。

> 虽然该平台能够并且应该继续作为一个开发人员友好的环境蓬勃发展，但有一些应用程序(不属于该平台的一部分)我们必须确保 Android 的安全模式完好无损。
> 
> “确保”是由 Android Pay 甚至第三方应用程序通过 SafetyNet API 完成的。正如你们可能想象的那样，当涉及到支付凭证和(通过代理)真金白银时，像我这样的安全人员会变得格外紧张。我和我在支付行业的同行花了很长时间，努力研究如何确保 Android Pay 在一个设备上运行，该设备有一套记录良好的 API 和一个很好的安全模型。
> 
> 我们的结论是，Android Pay 做到这一点的唯一方法是确保 Android 设备通过兼容性测试套件，其中包括对安全模式的检查。早期的谷歌钱包点击支付服务结构不同，让钱包能够在支付授权前独立评估每笔交易的风险。相比之下，在 Android Pay 中，我们与支付网络和银行合作，对您的实际卡信息进行令牌化，并仅将此令牌信息传递给商家。然后，商家像传统的卡购买一样清算这些交易。我知道你们中的许多人都是专家和超级用户，但需要注意的是，我们真的没有一种好的方法来向整个支付生态系统阐明特定开发人员设备的安全细微差别，或者确定您个人是否可能采取了特定的攻击对策——实际上许多人都不会。-[jasondcrington _ Google](http://forum.xda-developers.com/member.php?u=6957306)，谷歌[的安全工程师在我们的论坛上发言](http://www.xda-developers.com/google-security-engineer-explains-issues-with-root-and-android-pay-in-the-xda-forums/)

幸运的是，XDA 总能找到办法(尽管这次是无意的)。在不修改/system 分区的情况下启动你的设备。无系统根由 XDA 资深公认开发者和开发者管理员 [Chainfire](http://forum.xda-developers.com/member.php?u=631273) ，用户能够绕过根限制[访问 Android Pay](https://www.reddit.com/r/Android/comments/3qu3zk/chainfire_systemless_root_experiment/cwiezgg) 。然而，在一篇 Google+帖子中，Chainfire 提到这一“修复”仅仅是*“偶然的，而不是设计的，Android Pay 将会更新以阻止它。”看起来谷歌终于介入并更新了他们的 SafetyNet API，在无系统的根方法发布 91 天后。*

你好，黑暗，我的老朋友

在 Reddit 和 T2 我们自己的论坛上流传着几份报告，称最新的安全网检查检测到无系统的 root，这意味着你不能再在有 root 的设备上使用 Android Pay。如果你是一个 Android Pay 用户，你的设备使用了无系统根方法，那么你可能会注意到应用程序仍然为你打开，你会否认(我知道，这很难承认...)但不幸的是这是真的。Android Pay 只会在首次安装和打开应用程序时、添加新卡时以及交易时检查您的设备是否通过兼容性设备套件。我们论坛上的用户注意到，该应用程序可能会给你一个绿色的复选标记，诱使你错误地希望它可以工作，但唉，不，交易不会再处理了。

然而，并不是所有的都失去了。幸运的是，在购买之前，您可以从 SuperSu 应用程序中禁用 su，以暂时允许您的设备通过 CTS 检查。完成购买后，您可以打开 SuperSu 应用，[忽略“更新二进制文件”弹出窗口](http://forum.xda-developers.com/showpost.php?p=65053125&postcount=250)，并重新启用 Su。当然，这有点不方便，但至少你在手机上购物的时候还能享受你的~~暴露模块~~广告拦截器。

*更正:x 暴露的模块仍然会触发 CTS 检查，因此在使用 Android Pay 之前，您还必须禁用 x 暴露。*