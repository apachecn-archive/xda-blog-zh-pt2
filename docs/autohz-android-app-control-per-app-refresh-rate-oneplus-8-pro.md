# AutoHz 可让您控制一加 8 和一加 8 专业版上每个应用的刷新率

> 原文：<https://www.xda-developers.com/autohz-android-app-control-per-app-refresh-rate-oneplus-8-pro/>

一加是少数几家同时拥有 120Hz 高刷新率显示器的原始设备制造商之一，同时也允许在面板上设置最高 QHD+分辨率。然而，即使是最大 120Hz 的设置也不是在所有应用中统一设置的——正如一加指出的，“刷新率将根据场景动态切换”。一加没有明确提到一加 8 Pro 的刷新率将降低的场景，但我们从一加 7 Pro 的 AMA 上的[得知，这款手机使用可变刷新率来降低刷新率，用于观看视频、使用相机应用程序和打电话等场景。如果你想在每个应用程序的基础上更好地控制刷新率，XDA 认可的开发者](https://www.xda-developers.com/oneplus-7-pro-usb-pd-hdmi-variable-refresh-rate/) [arter97](https://forum.xda-developers.com/member.php?u=4898097) 的 [AutoHz](https://play.google.com/store/apps/details?id=com.arter97.auto90) 应用程序可以让你为你手机上的每个应用程序设置刷新率。

在股票一加设置中，60Hz 模式选项使设备像大多数其他智能手机一样以恒定的 60Hz 运行。90Hz/120Hz(取决于最大刷新率)模式选项实际上充当“自动”选项，在某些条件下将刷新率切换回 60Hz。有一个隐藏的*真* 90Hz/120Hz 设置，您可以通过 ADB 命令启用[，但这会增加您设备的功耗，即使在这种情况下您不一定会受益于更高的刷新率。对于 90Hz，Dylan 测量的功耗增加约为 30mW 小时，或者仅用于显示器的一加 7 Pro 每小时总电池额外增加约 0.5%，并且很可能有来自 SoC 和 GPU 的额外功耗来推动每秒这么多帧。](https://www.xda-developers.com/oneplus-7-pro-true-90hz-display-mode/)

这就是 AutoHz 的用武之地。我们在过去报道过 AutoHz，[回到它被称为 Auto90](https://www.xda-developers.com/auto90-control-oneplus-7-pro-display-refresh-rate-giveaway/) 的时候。从那时起，该应用程序已经扩展了对多种一加设备的支持，将其扩展到 90 赫兹的一加 8 和 120 赫兹的一加 8 Pro。该应用程序可让您控制一加设备切换到 60Hz 或 90/120Hz 的方式和时间，或者让它自动决定。该应用程序专为具有高刷新率显示器的一加设备(即一加 7 专业版、一加 7T、一加 7T 专业版、一加 8 和一加 8 专业版(120 赫兹))制作，仅适用于 OxygenOS。该应用程序也需要与亚行一次性设置。

在应用程序中，您会看到已安装应用程序的列表和每个应用程序旁边的切换按钮。60Hz 设置将该应用程序内的显示频率设置为 60Hz，90/120Hz 设置将该应用程序内的显示刷新率设置为 90/120Hz，自动设置保持该特定应用程序的系统默认行为。注意，对于一加 8 专业版，没有 90Hz 的中间设置-所以你可以选择 60Hz 或 120Hz。该应用程序已经包含一些常用应用程序的推荐设置，但它可以让您行使完全控制。

### AutoHz 应用的赠品

AutoHz 是一个付费应用程序，所以不是每个用户都愿意为在性能和电池之间找到平衡而付出代价。出于同样的原因，**我们将随机向我们的读者发放 20 个促销代码**。~~要获得该应用的推广代码，只需在下面的评论部分输入您的 XDA 论坛用户名。我们将在 24 小时后再次检查，在随机列表选择器中输入用户名，并将促销代码发送到您的论坛个人资料中。本次赠品不接受其他形式的参赛。~~ **赠品已经结束。**

* * *