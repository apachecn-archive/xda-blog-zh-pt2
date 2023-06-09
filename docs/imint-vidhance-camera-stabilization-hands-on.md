# Imint 的 Vidhance 软件的实践:强大的视频稳定！

> 原文：<https://www.xda-developers.com/imint-vidhance-camera-stabilization-hands-on/>

即使你认为自己非常了解智能手机领域正在发生的事情，你也很可能以前没有听说过像 Imint 这样的公司。并非每家智能手机公司都能像苹果、三星或华为一样，在内部开发几乎所有自己的技术，甚至我们刚刚提到的三大智能手机公司也仍然经常从第三方获得技术许可。Imint 就是这样一家为智能手机制造商开发软件并向其授权的公司，其中许多制造商你可能很熟悉，包括华硕、摩托罗拉、小米、Vivo、华为、一加、OPPO、HMD Global 等等。该公司的标志性 Vidhance 套件由各种相机技术组成，实现了我在任何手机上见过的最佳稳定性。

Imint 是一家成立于 2007 年的瑞典公司，目前开发并授权了 [Vidhance SDK](https://weareimint.com/products/sdk/) ，这是一个软件开发套件，用于芯片组供应商和智能手机设备制造商集成 Imint 的视频增强技术。早在二月份，艾明特宣布了他们的 Vidhance 软件套件的两个新成员:[自拍模式和超级稳定](https://www.xda-developers.com/vidhance-selfie-mode-mutli-camera-imint/)。自拍模式旨在当您从前置摄像头录制视频时，将您的面部保持在帧中，而超级稳定使用广角和高分辨率摄像头来稳定视频中的过度运动。这两个功能都经过了优化，可以在高通骁龙 865 的 [Spectra 480 ISP 上运行，并且它们都已经在新的摩托罗拉 Moto Edge+](https://www.xda-developers.com/imint-qualcomm-optimize-video-enhancement-snapdragon-865/) 上运行[。](https://www.xda-developers.com/motorola-edge-plus-first-phone-imint-new-vidhance-stabilization-tech/)

为了演示 imit 的 Vidhance 软件，imit 给我发了两台运行定制版 Android 的 Pixel 2 设备，其中嵌入了 imit 的软件。这两款手机预装了 3 个不同的应用程序:稳定、Live Composer 和自动分区。在下面的视频中，我浏览了不同的选项，展示了一些设置，并对每个应用程序进行了演示。

**稳定**当然是为了产生超级稳定的视频。启用它后，我发现视频稳定性比手机单独的 OIS 好得多。(由于发给我的两款手机都运行的是经过修改的 AOSP ROM，我无法测试标准的谷歌相机应用程序与谷歌的融合视频稳定[OIS+EIS]进行比较。)尽管如此，结果还是不言自明:Vidhance stabilization 在稳定后置摄像头的视频方面做得非常出色。前置视频在这种情况下更加令人印象深刻，因为在许多手机上，前置摄像头上没有 o is。这意味着如果没有任何软件稳定，前置视频会变得非常不稳定。

接下来是**自动分区**，这是我认为最令人印象深刻的功能。通过自动分区，您可以对特定区域进行分区，并在移动相机时保持该区域的焦点对准。例如，你可以在公园里移动你的手机，但是只要你选择的区域在相机的视线范围内，它就会一直在那个区域被裁剪。

接下来是 **Live Composer** ，基本允许超平滑缩放。虽然这听起来没什么大不了的(实际上也不是)，但它是*真正的*灵巧的玩法。当你意识到在大多数智能手机上放大会有多不稳定时，你会大吃一惊。

虽然所有这些功能看起来都令人印象深刻，但请记住，它们不只是供您通过应用程序下载的。Imint 授权原始设备制造商在其智能手机中使用这项技术。也没有简单的方法来判断 Imint 的哪些 Vidhance 功能正在任何特定的智能手机上使用，因为原始设备制造商通常不会费心(或者更确切地说，不愿)列出他们正在许可的技术。至少对于摩托罗拉 Moto Edge+，我们知道它支持几个新的 Vidhance 功能，包括视频稳定，水平校正，动态模糊减少和视野校正。尽管我还没有机会在商用设备上尝试这些功能，但我在 Imint 借给我的演示 Pixel 2 上看到的东西给我留下了深刻的印象。