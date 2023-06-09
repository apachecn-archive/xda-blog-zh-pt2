# Microsoft Exchange Server 用户正成为 Hive 勒索软件攻击的目标

> 原文：<https://www.xda-developers.com/microsoft-exchange-server-users-hive-ransomware-attack/>

每隔一天，似乎都有关于微软产品的重大安全问题的新闻报道，而今天，似乎微软的 Exchange Server 成为了另一个产品的中心。微软 Exchange Server 客户正成为 Hive 实施的一波勒索软件攻击的目标，Hive 是一个知名的勒索软件即服务(RaaS)平台，目标是企业和各种组织。

该攻击利用了 Microsoft Exchange Server 中一组称为 ProxyShell 的漏洞。这是一个严重的远程代码执行漏洞，使得攻击者能够在受影响的系统上远程运行代码。虽然 ProxyShell 保护伞下的三个漏洞在 2021 年 5 月得到了修补，但众所周知，许多企业并没有像他们应该的那样经常更新他们的软件。因此，各种客户都受到了影响，包括一位与 Varonis Forensics 团队交谈过的客户，该团队首先报告了这些攻击。

一旦利用了 ProxyShell 漏洞，攻击者就会在目标 Exchange 服务器上的公共目录中植入一个后门 web 脚本。然后，该脚本运行所需的恶意代码，然后从命令和控制服务器下载额外的 stager 文件并执行它们。然后，攻击者创建一个新的系统管理员，并使用 Mimikatz 来窃取 NTLM 哈希，这使他们能够通过哈希传递技术在不知道任何人的密码的情况下控制系统。

一切就绪后，心怀不轨的参与者开始扫描整个网络，寻找敏感和潜在的重要文件。最后，创建并部署一个定制的有效负载——一个名为 Windows.exe 的文件——来加密所有数据，清除事件日志，删除卷影副本，并禁用其他安全解决方案，使其不被检测到。一旦所有的数据都被加密，有效载荷就会向用户显示一个警告，敦促他们付钱取回数据并保证数据的安全。

蜂巢的运作方式是，它不只是加密数据，并要求赎金归还。该集团还运营着一个网站，可以通过 Tor 浏览器访问，如果公司不同意付费，可以在那里共享公司的敏感数据。这给希望重要数据保密的受害者带来了额外的紧迫感。

根据 Varonis Forensics 团队的报告，在一个特定的案例中，从最初利用 Microsoft Exchange Server 漏洞到攻击者最终达到他们想要的目标只花了不到 72 小时。

如果您的组织依赖于 Microsoft Exchange Server，您需要确保安装了最新的补丁程序，以抵御这波勒索软件攻击。考虑到漏洞通常会在补丁发布后暴露，让过时的系统成为攻击者攻击的目标，因此尽可能保持最新通常是一个好主意。

* * *

来源:[瓦罗尼斯](https://www.varonis.com/blog/hive-ransomware-analysis)

Via: [ZDNet](https://www.zdnet.com/article/hive-hackers-are-exploiting-microsoft-exchange-servers-in-ransomware-spree/)