# Rovo89:牛轧糖 Xposed 的开发更新

> 原文：<https://www.xda-developers.com/rovo89-updates-on-the-situation-regarding-xposed-for-nougat/>

我个人继续在我的 [OnePlus 3](http://forum.xda-developers.com/oneplus-3) 上使用 Android 6.0 棉花糖的原因是 Xposed 的存在，尽管[一加为手机推出了牛轧糖更新](https://www.xda-developers.com/oxygen-os-4-0-2-and-new-open-betas-released-for-the-oneplus-3-and-3t/)。Xposed 框架和模块生态系统构成了我更喜欢的 Android 体验的一个重要部分——以至于我愿意放弃来自 OEM 的最新操作系统更新，只为了品尝这个甜蜜的果实。

虽然牛轧糖的发布需要一段时间，我们中的一些人不介意再等一会儿，但自从我们上次听到这个项目的进展以来，已经有一段时间了。

XDA 资深公认开发商 [rovo89](https://forum.xda-developers.com/member.php?u=4419114) 花了一些时间[告知我们](https://forum.xda-developers.com/showthread.php?t=3034811&page=5)关于牛轧糖项目的当前情况:

“似乎越来越多的人开始担心牛轧糖是否会(以及何时)上市，所以我觉得我应该说点什么。

为什么要花那么长时间？因为在每个版本中，我都努力确保 Xposed 与新的 ART 版本中的改进很好地集成在一起。从棒棒糖到棉花糖这一步并不大。这是一种进化，有些东西甚至使得以更优雅的方式集成 Xposed 成为可能。总的来说，这主要是谨慎的移植，而不是创新。

牛轧糖改变了一些基本的东西。如果你已经在用牛轧糖了，你会发现现在安装速度快多了。这是因为 apk 不会立即编译(AOT)，而是以(较慢的)解释模式开始。听起来很糟糕，但他们已经启用了 JIT，这将快速编译那些经常使用的方法。这将恢复众所周知并不断提高的本机代码性能。除此之外，ART 还保留了这些常用方法的列表(“剖析”)。当设备空闲时，它最终进行 AOT 编译，但是基于分析数据。之后，您可以在启动应用程序后立即获得出色的性能。JIT 仍在等待，以防使用模式发生变化，我认为它也会调整配置文件并改进 AOT 编译。

这导致了各种不同的编译状态和更多的复杂性。除此之外，Xposed 需要重新编译整个 ROM 和所有应用程序，这在过去引起了许多问题:当 odex 文件被过度预优化时，它有时会导致引导循环，它阻塞了相当多的存储空间来存储重新编译的文件，我需要禁用一些优化，如内联和直接指针调用。我希望我可以利用 JIT 编译器来避免在牛轧糖中出现这种情况。如果 Xposed 知道从哪里调用方法，它可以使调用者编译的代码无效，这样他们就可以暂时使用解释器。如果它们足够重要，JIT 会重新编译它们。

我已经为此做了大量的研究和实验，目前我正在尝试实现它。但是你可以想象，所有这些都需要很大的努力，很容易就要花费数百个小时.....”

业余爱好者项目中的主要问题通常是时间的分配，我们知道 rovo89 来自哪里。即使是目前的 Xposed 项目，它也包含了各种开发人员数月的努力，以帮助最终用户以如此简单和可分发的方式享受。

正如人们所说，罗马不是一天建成的，而是每小时都在砌砖:

> 所以是的，我还在做牛轧糖支持，只要我的空闲时间允许，但我不知道什么时候会完成。一旦完成，你就知道了。

Android 并不完美，这让我们可以修复原始开发者不愿意做的事情。对最新操作系统的最终 Android 补丁的等待仍在继续，我们希望 rovo89 在我们这边好运。

**你可以在[论坛帖子](https://forum.xda-developers.com/showthread.php?t=3034811&page=5)中阅读完整声明。你也在等着曝光吗？请在评论中告诉我们！**