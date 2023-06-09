# doubleTwist 音乐播放器评论

> 原文：<https://www.xda-developers.com/cloudplayer-diy-hifi-music-streaming-solution/>

在我们的[音乐流媒体服务](http://www.xda-developers.com/a-helpful-guide-to-music-streaming-services/)实用指南中，我们提到了几种不同的服务，它们提供了将音乐目录直接传输到你的设备的方法。虽然每种服务都有其优点和缺点，但它们的共同主题是让您可以访问庞大的音乐库，而无需存储自己的音乐库，并为此收取月费。但是如果你已经有了自己的音乐目录呢？当然，有很多音乐锁服务可以让你上传和播放你自己的文件。Google Play Music 允许你免费上传多达 50，000 首歌曲，当你在物理介质上购买音乐时，亚马逊音乐甚至可以自动为你存储这些歌曲。但是，如果您想绕过这些服务对您的文件进行的重新编码，该怎么办呢？如果您想使用已经付费的云存储服务，该怎么办？进入开发者 doubleTwist 的最新应用 CloudPlayer。

简单来说，doubleTwist 的 CloudPlayer 允许你使用你已经使用的云存储服务，从你已经拥有的文件中构建你自己的音乐流媒体服务。该应用程序链接到你的 Dropbox、OneDrive 和 Google Drive 账户，并从本地存储中提取数据，扫描每个账户的兼容媒体。然后，它从所有可用的来源构建一个数据库，并将其组织到一个音乐库中，包括专辑封面、标签和元数据。  支持 MP3、AAC、OGG、M4A、WAV、WMA 文件，从 1.0.4 版本开始，还支持 FLAC 文件，包括更高分辨率的文件(最高 24 位，192kHz 音频)。这可能是使用 CloudPlayer 而不是其他数字音乐锁服务的最大原因，因为大多数其他人会将无损或高分辨率文件重新编码为某种有损格式。您可以随时让任何文件或播放列表可供离线播放，并将所需的数据限制为仅传输到 WiFi 网络。还有 Chromecast 和苹果 AirPlay 支持，最后。FM scrobbling 是内置的。

CloudPlayer 是从谷歌 Play 商店免费下载的，但是需要一次性购买 4.99 美元的应用程序才能解锁最想要的功能，包括云存储功能本身、Chromecast 和 AirPlay 支持，以及均衡器和其他声音处理功能。第一次打开应用程序时，你会看到这些信息，并可以通过使用谷歌帐户登录，免费试用这些“高级”功能 7 天。

[![CloudPlayer_FreeTrial](img/e16bf32d707e9dfc6c08cdf7aa492657.png)](http://www.xda-developers.com/wp-content/uploads/2015/07/Screenshot_2015-07-28-22-48-17.png)

该应用本身从 Google Play 音乐中借鉴了许多视觉和操作上的线索，这并不是一件坏事。它提供材料设计，并围绕着一个基于手势的界面来导航你的音乐库。汉堡菜单弹出，并允许快速方便地访问排序选项，如专辑，艺术家，播放列表，歌曲，流派和作曲家。在这里，您还可以仅显示您下载用于离线回放和存储在本地的曲目，以及访问设置菜单。从“设置”菜单中，您可以链接到或重新扫描您的云存储服务，包括 Dropbox、OneDrive 和 Google Drive，打开或关闭蜂窝数据的使用，更改默认排序选项，设置 Last.fm scrobbling 或重置音乐数据库。

一旦连接您的云存储帐户并允许 CloudPlayer 访问它们，就会使用曲目元数据和专辑封面来构建和组织数据库。在浏览曲库时，溢出菜单可用于使曲目或选择离线可用、添加到现有或新的播放列表、添加到播放队列或删除。选择要播放的内容会将你带到正在播放屏幕，或者你可以从底部向上滑动它，从应用程序的任何地方访问它。该屏幕布局合理，功能强大，包括高质量的专辑封面、播放/上一张/下一张按钮、随机播放和重复控制、以“曲目名称-艺术家姓名”格式滚动的标题栏，以及已播放/剩余曲目时间。您可以在专辑封面上左右滑动来快速浏览播放列表，或者轻按专辑封面来评价当前播放的曲目。正在播放屏幕的底部有一个“下一个”部分，允许你查看和快速跳转整个播放列表。溢出菜单按钮调出 10 波段均衡器、超声设置(耳机的模拟环绕声设置)、浏览当前播放的艺术家、浏览当前播放的专辑和清除播放队列选项。

该应用程序支持锁屏控制，全屏显示专辑封面，还具有快速控制的持续通知。还有三个主屏幕小部件:一个完整的 4x4 小部件和两个 4x1 小部件:一个深色主题的小部件和一个浅色主题的小部件。

性能流畅快速，在应用程序中导航时不会出现可检测到的口吃或丢帧现象。我从任何受支持的云存储服务中播放 MP3 和 FLAC 格式的文件都没有问题，但请记住，当应用程序访问曲目并缓冲它时，会有一两秒的轻微延迟。我唯一一次注意到明显的延迟是当我快速跳过一首歌很多次，迫使它完全重新缓冲时，但这对大多数人来说应该不是问题。

有一些值得注意的功能缺失了，例如缺乏交叉渐变或无间隙播放支持，缺乏对存储在 Google Drive 上的音乐的 ChromeCast 支持，无法添加或编辑曲目元数据或专辑封面，以及无法直接从应用程序中将音乐从您的设备上传到云。然而，这些功能在 Play Store 的描述中都被列为即将推出。我希望看到的一个缺失特性是能够查看任何类型的文件信息，比如音频文件的类型、比特率、采样率和位深度信息。现在，如果你的音乐库中有混合的文件类型或质量，你将无法区分它们。然而，CloudPlayer 是一个相对较新的应用程序，所以我们可以肯定 doubleTwist 正在努力增加功能，并在可预见的未来保持对应用程序的良好支持。

尽管缺少功能和 4.99 美元的价格，CloudPlayer 在它想要实现的目标上表现出色。能够连接到多个云存储服务的好处意味着，人们可以只使用三个服务中的每一个服务提供的免费存储空间来支持一个相当大的音乐库，而不必只为其中一个服务支付每月存储费用。虽然 Google Play Music 和 Amazon Music 本身是很好的服务，但你无法从它们那里获得无损音频流，因为它们都将上传内容重新编码为有损文件格式。doubleTwist 在这里发布了一个非常有能力、设计良好、表演出色的音乐播放器，他们对音乐流的处理会让很多人非常满意。

你可以从[游戏商店](https://play.google.com/store/apps/details?id=com.doubleTwist.cloudPlayer)买到 doubleTwist 的 CloudPlayer。

你也可以从 doubleTwist 的[产品页面](https://www.doubletwist.com/cloudplayer)了解更多关于 CloudPlayer 的信息。

* * *

你试过 CloudPlayer 或其他音乐寄存服务吗？请在评论中告诉我们你的印象！