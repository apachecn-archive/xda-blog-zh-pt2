# 谷歌为 Android Q 备受争议的手势导航辩护

> 原文：<https://www.xda-developers.com/google-defends-android-q-gesture-navigation/>

Android Q 的公开发布指日可待，届时我们将看到来自终端用户的大量反馈，他们将首次尝试手势导航功能。手势导航系统是近年来 UX 最大的变化，因为它们从根本上改变了用户在操作系统中的导航方式。用户现在需要从左/右边缘向内滑动才能向后导航，从底部边缘向上滑动才能跳转到主屏幕，从底部角落向内滑动才能触发虚拟助手。到目前为止，这些姿态已经招致了用户的很多赞扬[和批评](https://www.xda-developers.com/google-android-q-gesture-mess/)，本质上是基于用户偏好来划分社区。在 Android 开发者博客上的一篇新文章中，谷歌为 Android Q 上的手势导航进行了辩护，并试图解释各种相关决定背后的基本原理。

谷歌决定尝试手势是受到 Android 合作伙伴越来越多采用这些手势的启发，以及创新的 Android 应用程序，如[我们自己的导航手势应用程序](https://www.xda-developers.com/navigation-gestures-1-11-7-changelog/)(谷歌在博客帖子中提到过)。手势被认为比软件按钮更快、更自然、更符合人体工程学。与可能被意外触摸的软件按钮相比，它们需要更强的调用意图。此外，手势为应用程序和其他内容留出了大量屏幕空间，这符合更大屏幕和更小边框的大趋势。

但是，随着这些积极因素的陈述，谷歌也意识到手势不会引起每个用户的相同反应。它们可能更难学习，需要有意识的努力来改变肌肉记忆。在某些情况下，它们还会干扰应用程序中的导航模式。此外，谷歌手势的最大问题是每个 OEM 厂商实现手势的方式不同，导致导航体验的碎片化。从谷歌的角度来看，这是一个大问题，因为它在导航这样的核心主题上导致了不同的操作系统体验，影响了用户和开发者。

由于这种碎片化，Android Q 的手势将成为新 Android Q+设备的[默认手势导航。这一决定是与谷歌与三星、小米、Oppo、HMD Global、一加、LG、摩托罗拉等合作伙伴共同努力实现导航体验标准化的结果。然而，由于这些手势并不适合所有人，尤其是那些灵活性和移动性有限的人，这些手势将与一个选项共存，以便为软件按钮启用三按钮导航栏。](https://www.xda-developers.com/android-q-navigation-gestures-mandatory/)

然后，谷歌进一步为继续使用当前手势的决定辩护，提到他们的所有决定都是由对整个主题的广泛研究和测试支持的。当前实现中的两个核心手势 Back 和 Home 被设计为与拇指最容易到达和最舒适的运动区域相一致。

 <picture>![](img/f60b78ed6af3517d79cbb81c99f2fbc7.png)</picture> 

Phone screen heatmaps showing where users can comfortably do gestures, holding the phone in only one hand

Android Q 的手势导航是在测试了其他几个导航实现和原型之后推出的。在这些测试的结论中，用户认为 Android Q 的模型更适合单手使用。

谷歌确实指出，Android Q 手势会干扰应用程序抽屉和应用程序内的其他滑动。但鉴于 Back 的大量使用，谷歌最终做出了艰难的决定，要求开发者解决与系统手势的冲突。为了促进这一过程，Google 提供了额外的资源，详细说明了开发人员可以采用的良好实践。如果你的应用本身使用了基于手势的导航，我们建议你通读谷歌在他们的文章底部提到的资源。手势导航是前进的方向，所以我们最好适应。

* * *

**来源:[安卓开发者博客](https://android-developers.googleblog.com/2019/08/gesture-navigation-backstory.html)**