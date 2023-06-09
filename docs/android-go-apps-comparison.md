# Android Go——Google 的轻量级生态系统与原版相比如何？

> 原文：<https://www.xda-developers.com/android-go-apps-comparison/>

Android Go 是谷歌的轻量级移动平台，旨在运行在比通常更低的系统规格上。它的目标是发展中国家和低收入地区，在这些地区，处理器性能差、内存容量小的设备将最为普遍。它的存在基本上是为了确保发展中国家的用户仍然可以利用智能手机领域的应用程序和产品。因此，较低的规格要求重新设计一些应用程序，以便在更小的 RAM 限制内工作。YouTube Go、Maps Go、Gmail Go 和 Google Go 都是这些应用程序的例子，第三方也提供这些应用程序。但这还不是全部，还做了许多修改以保持系统要求更低。RAM 压缩、减少的系统内存使用和更好的内存管理确保了设备尽可能快地运行。

但就智能手机而言，它的价值取决于它能运行的应用程序。目前可用的 Android Go 应用套件到底有多好？我们将预装的 Android Go 应用程序与正常的应用程序进行比较，以找出答案。

## 安卓 Go vs 普通安卓——怎么回事？

操作系统之间有什么区别？在一个未修改的 Android Go 版本上，很少。有趣的是，Android Go 与其成熟的同类产品非常相似，并不像 Android One 计划中的那样直接发布到 Android 设备上。该软件被运送到手机制造商那里，然后他们对其进行修改并添加他们自己的应用程序和软件。即将推出的三星 Android Go 设备就是一个例子。几乎所有 Android Go 的变化都隐藏在普通用户在日常使用中不会看到的东西。然而，理论上，没有什么可以阻止 OEM 厂商更进一步，做出更多的改变。还是很熟悉，感觉还是一样，这才是重点。这个系统有一些小的变化，但没有什么显著的变化。我唯一能发现的 UI 变化是最近的应用程序是如何显示的，如下所示。在我的测试设备上，我无法发现两者之间有任何其他重大差异，因为谷歌的愿景是这两个操作系统在功能上保持一致。

*左:安卓 Go //右:安卓*

有趣的是，最近的应用切换器的变化旨在“欺骗”用户。当应用程序加载时，缩略图会扩展到整个屏幕，这在分辨率较低的设备上并不明显。这是一个巧妙的小技巧，让这个设备看起来比实际更快。

有一些功能被禁用，但没有一个是给定平台的主要功能。分屏和 Daydream VR 一起被禁用。考虑到内存和屏幕分辨率的限制，这两种情况都是完全可以理解的。这里也没有 Android Auto 或 Wear OS 支持，并且 Android for Work 配置文件被禁用。默认情况下也没有加密，但有些设备会允许你重新打开它。

到目前为止，谷歌已经让 Android Go 和他们的应用程序套件完美下线。现在，要延续这一趋势，就要靠各个手机制造商和应用开发商了。

在其他功能方面，谷歌的精简版 Android 几乎完美地复制了它的大兄弟。这里没有太大的区别，尽管它减少了 RAM 的使用和存储空间。Android Go 也非常重视保护你的数据使用，但没有什么是你在标准的 Android 旗舰智能手机上找不到的。我们已经深入讨论了这些变化。

Android Go 在清除低优先级进程方面要积极得多，所以基本上，任何与后台运行的 Android 系统无关的东西。自动存储管理也出现了，通过修剪一些不需要的功能的系统服务，减少了 Android 系统内存。

有趣的是，Android Go 的许多内置应用程序都被美化为渐进式网络应用程序，这是谷歌已经研究了一段时间的东西。

## Gmail Go vs Gmail

*Gmail Go*

Gmail Go 主要关注功能，这也是普通 Gmail 所关注的。它拥有精简形式的电子邮件应用程序所需的所有功能，看起来与更完善的版本几乎一样。

*Gmail*

正如你所看到的，Gmail 在图形方面比 Gmail Go 领先很多。帐户切换器有一个很好的动画，你可以滑动，而不只是一个切换下拉菜单。电子邮件撰写活动还在顶栏和实际撰写区域之间有一个阴影，这是该应用程序的简化版本所缺少的细节。

那么有什么区别呢？除了微小的视觉变化外，并没有太大的变化。该应用程序的功能是相同的，并且做的正是您期望电子邮件客户端做的事情。这里没有遗漏任何功能。不过，性能方面则完全不同。Gmail Go 使用网络视图，因此性能不稳定。这里的主要问题是，谷歌更关注保持文件大小，而不是优先考虑性能，因为一个基本的电子邮件客户端不需要运行良好。有趣的是，Gmail Go 的文件大小实际上比 Gmail 大。在这里，你最好使用普通版的 Gmail。

## YouTube Go vs YouTube

*YouTube Go*

YouTube Go 与 Gmail Go 处于同一条船上，因为它主要关注简单性和易用性，同时也让用户了解文件大小。一个视频将使用多少数据是明确概述的。没有评论，不能喜欢或不喜欢视频。您可以在播放视频之前阅读其描述。这款应用程序提供了与普通 YouTube 应用程序截然不同的体验，即使用户界面和设计语言基本保持不变。

*YouTube*

与普通的 YouTube 应用程序相比，YouTube Go 看起来更简单，功能更少。它能完成工作，但就是不够健壮。我还遇到了 YouTube Go 的奇怪性能问题，这些问题在普通的 YouTube 应用程序中并不存在。例如，当我播放一个视频并向下滚动到推荐的视频时，有一秒钟左右的时间，设备一直处于静止状态。非常奇怪的东西。尽管如此，YouTube Go 作为观看 YouTube 视频的客户端功能非常完美，在其他方面也做得非常好。它之所以变得更好，是因为它让用户保持数据意识。

## 谷歌围棋和助手围棋 vs 谷歌

现在，这是事情变得非常不同非常快。**这两个应用程序根本没有可比性**。Google Go 感觉像是一个完全不同的应用程序，从某种意义上来说，我想是的。为了便于比较，我将 Assistant Go 和 Google Go 结合在一起，因为常规的 Google 应用程序包含了两者的功能。有趣的是，当我的设备语言设置为英语(爱尔兰)时，它不让我通过 Assistant Go 使用谷歌助手。我不得不把它改成英语(英国)。这个限制在完整版中不存在。

*Google Go*

Google Go 类似于常规的 Google 应用程序，但有一些令人惊讶的额外功能。这里有趋势搜索和许多定制选项。挺酷的。Google Go 绝对是目前最好的 Android Go 应用之一。它拥有你需要的谷歌应用程序的所有功能，并且有一个好看的用户界面。唯一的问题是你不会得到推荐的新闻卡片。

 <picture>![](img/bc0924a71514cd43dfe052eb75f40daa.png)</picture> 

*Google*

常规的 Google 应用程序显然更好，但 Google Go 的制作令人惊讶地好，而且做得很好。至于助手 Go 应用程序，它几乎只是从谷歌应用程序中取出的助手，并将其制作成自己的东西。有一两个限制，比如绝对没有配置选项，但是工作原理基本一样。例如，你可以告诉它在 Spotify 上播放音乐，但你不能告诉它设置默认音乐播放器。它也不能控制手机的硬件，比如打开手电筒。但是所有的基本功能都工作正常。

在 UI 方面甚至没有太多变化，所以如果你换成基于 Android Go 的智能手机，它会像往常一样熟悉。据我所知，没有任何功能被遗漏。我的所有请求都工作得很好，就像在常规助手中一样。你会发现唯一的大区别是没有“Ok Google”热词检测，这是可以理解的，因为它没有像在常规 Android 设备上那样被纳入系统。

## 谷歌地图 Go vs 谷歌地图

这是谷歌真正需要做出一些改变的地方，以使他们的地图应用程序能够在低内存设备上工作。事实上，许多旗舰设备在运行完整版谷歌地图时会出现延迟或口吃。这是一个挑战，但谷歌让它在 Android Go 上工作，运行得很好(虽然不是很好，但它使用的 webview 就像 Gmail Go 一样)。感觉肯定是不同的，但是功能是一样的，而且它非常好地满足了你的需要。有趣的是，这也是我用过的最小的 Android Go 应用之一。它的大小不到 1MB，这可能是因为它是一个 webview，而不是一个成熟的应用程序。

*谷歌地图上线*

还记得我说过 Google Go 是迄今为止最好的 Android Go 应用之一吗？嗯，谷歌地图 Go 可能是*制作最精良的安卓 Go 应用。它无疑赢得了最准确娱乐的分数(除了助理围棋)。看看下面的普通版谷歌地图的截图吧——惊人的相似。*

*谷歌地图*

显然有一些图形差异，但没有太大，使它成为一个完全不同的应用程序。这是一个非常非常好的娱乐，让我印象深刻。当然，谷歌地图 Go 确实放弃了一些其他功能，如推荐优步或我的出租车，但这也没什么，因为这些基本上都是广告。我对这个应用程序完全没有问题，谷歌在重建它方面做得很好。不过，谷歌地图 Go 是一个有趣的例子，因为你可以在自己的 Android 设备上使用它，只需在智能手机上导航到谷歌地图网站。实际上是完全一样的东西。因此，有一个限制，但这可能是预料之中的——这里没有实时 GPS 逐路段导航。由于这一限制，你不能在开车时让手机告诉你方向。对于一些人来说，这可能是一个交易破坏者，但作为一个简单的地图应用程序，它对我来说非常完美。还有一两个其他功能也不见了，即评论，但我发现自己在谷歌地图中并没有太多地使用它们。

## 那么 Android Go 怎么样呢？

Android Go 目前处于一个有趣的位置。它拥有成为一个伟大的轻量级操作系统的所有潜力，同时在很多方面也没有达到目标。这是它的应用程序的总和，它的应用程序当然不是一流的。描述它们的唯一方式是不一致的，虽然单独来看它们还不错，但它们会让你觉得你在玩一个不完整的生态系统。话说回来，物有所值，对于大多数 Android Go 手机的标准价格来说，这当然没有什么错。可以理解的是，为了适应存储和处理的限制，一些应用程序不得不偷工减料。该系统非常适合那些寻找廉价二手手机或老年人手机的人。肯定不是给发烧友看的。