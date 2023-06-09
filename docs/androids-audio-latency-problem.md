# Android 的音频延迟问题

> 原文：<https://www.xda-developers.com/androids-audio-latency-problem/>

多年来，围绕 Android 和音频的结合一直存在明显的不安，这是可以理解的。我们[上个月](http://www.xda-developers.com/audio-focused-apis-mark-promising-direction-for-android/)发表了一篇文章，讲述了即将推出的 Android M 的变化会如何影响音频应用的实现，以及我们希望这对整个平台意味着什么，从那以后，我们发现了一些资料，使这一切背后的逻辑更容易理解。

真正支撑这一点的是 Android 中的音频延迟问题，尤其是与其他操作系统相比。对于那些不熟悉这个术语的人来说，延迟就是信号到达某一点(通常是一次往返)所需的时间。在流行文化中，你会发现它在在线游戏中被多次提及，其中延迟导致了玩家在共享游戏中体验到的输入和响应之间的“滞后”。在音频领域，最简单的描述就是音频信号进入设备，经过某种转换和处理，然后再返回的时间。

Android 从来没有考虑过低延迟问题。仅仅是因为它的设计方式，它不可能达到强大的音频处理应用程序或同步性至关重要的现场环境所需的延迟。这是发烧友非常清楚的事情，但对于普通用户来说，Play Store 中缺乏音频软件，尤其是与竞争对手 iOS 相比，这是显而易见的。一些制造商，如三星，甚至创建了自己的 API，以试图减少设备上的延迟，并取得了一些成功，但在这样做的时候，他们仍然将任何音频应用的商业范围限制在他们的产品上，阻止公司从一开始就投入时间开发软件。

为了在现实世界中证明这一点，[查看这篇文章](https://nervous.io/android/audio/2015/07/10/android-audio-latency/)以找到一个相当广泛的 Android 设备列表，以及这个音频之旅的延迟实际上是什么。这对于开发音乐应用的开发者来说是很有用的，至少我们可以看到随着操作系统的成熟，这一数字会有显著的增长。同样，Android M 应该会继续这一趋势，但目前还不清楚会有多少，而且就个人而言，我们怀疑它会成为游戏规则的改变者。

其次，如果你想知道为什么会这样的完整解释，请阅读这篇精彩的文章。它以详细但清晰的语气解释了音频信号的实际情况，以及它在操作系统中必须经历的许多阶段。要记住的一件事是，作者试图通过试图取代大部分或全部这一过程来推动他们自己的解决方案，但如果这被采纳并最终使消费者受益，那么我们都将受益。

希望在不太遥远的将来，这种担心会被否定，音乐家和制作人不会立即被推向装备相对更好的苹果阵营。谷歌需要把一些注意力放在 Android 的这一方面，因为它需要一些认真的工作来使它在这方面变得有竞争力，但谢天谢地，看起来 Android M 将是一个开始。

你能想象自己在未来使用 Android 作为音频设置的一部分吗？请在评论中告诉我们！