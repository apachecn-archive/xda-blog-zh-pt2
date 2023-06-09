# 谷歌将为 Pixel 2 XL 增加新的色彩模式，保修加倍

> 原文：<https://www.xda-developers.com/google-pixel-2-xl-warranty-color-mode/>

去年，第一代谷歌 Pixel 和 Pixel XL 使用了三星的 AMOLED 显示屏。当时，谷歌的目标是 NTSC 色域，而 Android 没有色彩管理，因此默认情况下所有颜色看起来都是饱和的。尽管该公司在开发者选项中提供了 sRGB 模式。在今年的第二代 Pixel 2 手机中，谷歌为 Pixel 2 和 Pixel 2 XL 选择了不同的有机发光二极管面板。虽然 Pixel 2 使用了与 2016 Pixel 非常相似的全高清三星 AMOLED 显示屏，但 Pixel 2 XL 使用了 LG 新的 WQHD+ (2880x1440) 18:9 纵横比的 P-有机发光二极管显示屏。

LG 自己的旗舰智能手机 V30 上使用了相同的显示屏(尽管可能不是完全相同的面板，因为据报道，这两款手机之间的颜色偏移是不同的)，但谷歌以不同的方式校准了 Pixel 2 XL 的显示屏。在 Pixel 2 手机发布后，我们已经看到用户对 Pixel 2 XL 的显示质量的多次投诉。这些投诉包括色彩柔和、mura 颗粒、黑色拖尾、色带、视角中严重的蓝色偏移以及[烧屏](https://www.xda-developers.com/google-pixel-2-xl-display-burn-issues/)。

现在，谷歌在 Pixel 帮助论坛上发布了一篇总结文章和一篇题为“深入了解 Pixel 2 XL 的显示器”的深入文章，对显示器质量投诉做出了回应。谷歌在文章中承认了一些对显示屏的抱怨，尽管不是全部。

* * *

## 谷歌将增加一个新的饱和色模式

根据谷歌的说法，用户对柔和颜色的感知是因为 Android Oreo 的颜色管理和默认的 sRGB 颜色配置文件。色彩管理是奥利奥的一项新功能，它使显示器理解色彩空间的概念，如 sRGB，P3 DCI 等。

Pixel 2 (95%)和 Pixel 2 XL (100%)上的显示器都支持 DCI-P3 色彩空间，这是一种宽色域。然而，由于奥利奥的色彩管理系统，所有原生内容都默认以 sRGB 为目标，包括网络内容。DCI-P3 色彩空间只有在应用程序被特别标记时才会显示给用户。例如，谷歌相机支持宽彩色，但谷歌自己的许多应用程序不支持。这意味着大多数应用程序都在 sRGB 进行渲染，这是行业标准的色域。

感觉柔和颜色的问题之所以出现，是因为到目前为止，有机发光二极管显示器默认具有饱和色。这是由于有机发光二极管天然的宽色域(比 sRGB 宽)和安卓在奥利奥之前没有色彩管理系统的结合。

三星和其他制造商在其旗舰智能手机中有 sRGB 模式。例如，三星多年前就推出了色彩校准基本模式。然而，默认情况下，这些 sRGB 模式不会被使用；饱和模式(如三星的自适应显示模式)被用作默认模式，在这种模式下，颜色相对于 sRGB 色域是饱和且不准确的。因此，使用默认显示模式的用户已经习惯了有机发光二极管显示器上的饱和色，回到 sRGB 的窄色域是一个极端的变化，尽管颜色客观上更准确。还值得注意的是，有报告称，一些 Pixel 2 XL 单元校准不正确，导致色彩饱和不足，即使对于 sRGB 显示器也是如此。

该公司发运的 Pixel 2 和 Pixel 2 XL 都带有 sRGB“活力”(饱和)模式，该模式为 sRGB 增加了 10%的提升，并向各个方向扩展，使其稍微更有活力。然而，这对于想要在 Pixel 2 XL 上获得饱和有机发光二极管外观的用户来说还不够，因此**谷歌现在宣布将为 Pixel 2 和 Pixel 2 XL 提供另一种颜色模式，这将恢复饱和有机发光二极管颜色外观**。

谷歌将在新的颜色模式中实现饱和的有机发光二极管颜色外观，方法是将所有显示的内容拉伸到原生 DCI-P3 颜色空间，即使它们没有专门标记为使用宽颜色。这将使所有颜色更饱和，但通过使它们饱和，它们会更不准确，就像三星手机上的自适应默认显示模式一样。**该公司表示，这是一种不受管理的配置，将使事情类似于原始像素如何操作**。它还补充说，这种颜色模式提供了选择，用户可以选择他们喜欢的颜色模式。

* * *

## 谷歌回应烧屏问题

谷歌对 Pixel 2 XL 的烧屏投诉做出了回应，称之为“差异老化”——这个术语既包括永久烧屏，也包括图像残留。它表示，广泛的测试表明，Pixel 2 XL 显示器的衰减特性与其他有机发光二极管显示器相似。该公司表示，调查从 10 月 22 日开始，也就是第一批烧屏投诉开始的那一天，已经确认老化符合高端智能手机的情况，“不应该影响 Pixel 2 XL 的正常日常用户体验。”

该公司表示，它使用软件来“保护用户体验”，并最大限度地延长有机发光二极管显示器的寿命。在其深入的文章中，该公司承认，“在使用专门的显示测试应用程序时，看到老化的证据可能令人担忧”，因此它正在采取措施通过软件来减少老化。

具体来说，在研究了设计 Pixel 2 XL 软件时为减少烧屏而采取的决定后，该公司表示，目前正在测试一个软件更新，旨在通过在 Pixel 显示器底部添加一个新的导航栏淡出功能来防止出现这一问题。[(此功能在 Android 8.1 开发者预览版中观察到)](https://www.xda-developers.com/android-8-1-oreo-developer-preview-features/)。此外，谷歌正在与更多的应用程序合作，使用一个**光导航条**，这是用户界面的一个变化。最后，该公司提到，这一软件更新将**将 Pixel 2 XL 上的亮度降低 50 尼特**，这“几乎察觉不到”。根据谷歌的说法，这将大大减少屏幕上的负载，而“观察到的亮度变化几乎察觉不到。”

该公司表示，新的饱和色模式、导航栏上图标的淡出、白色背景导航栏的使用增加以及最大亮度的降低将在未来几周内作为 Pixel 2 XL 的软件更新提供。

* * *

## 谷歌对蓝色调颜色偏移问题的回应

谷歌提到，Pixel 2 和 Pixel 2 XL 已经校准到 D67 (6700K)的白点，而不是 D65 (6500K)。这是一个有意的选择，因为根据该公司的说法，用户认为这样的屏幕更“新鲜”，即使它确实使显示屏略冷。

至于蓝色，该公司表示，这是显示器硬件所固有的，“只有当用户以锐角握住屏幕时才可见。”根据谷歌的说法，由于像素腔设计，所有显示器都容易受到偏离角度的某种程度的颜色偏移。由于用户喜欢更冷的白点，谷歌再次采用了蓝移的设计。这个回答并没有彻底解释为什么 Pixel 2 XL 在以一个角度观看屏幕时会出现更极端的蓝移。

* * *

## 谷歌为 Pixel 2 和 Pixel 2 XL 用户提供双倍保修

在同一份公告中，**谷歌还表示，它已经为 Pixel 2 和 Pixel 2 XL 用户提供了双倍保修。现在，这两款手机的所有者将获得**两年的保修**，因为谷歌相信它们“提供了卓越的智能手机体验”**

在一次更新中，该公司澄清说，已经从谷歌商店或授权零售商购买了 Pixel 2 或 Pixel 2 XL 的用户，他们的保修期将延长至两年。在第二年发生机械故障时，用户不再需要支付免赔额。但是，意外损坏仍然有免赔额。

至于优先照顾，计划的长度保持不变。如果用户已经购买了该计划并希望退款，他们可以在 30 天内获得购买 preferred care 的全额退款，或者在该时间段后的任何时间获得按比例退款。

* * *

[**来源 1:像素帮助论坛**](https://productforums.google.com/forum/#!topic/phone-by-google/FRyoLZZjXvo)

[**来源二:像素帮助论坛**](https://productforums.google.com/forum/#!topic/phone-by-google/y1FWSMFcDgA;context-place=forum/phone-by-google)