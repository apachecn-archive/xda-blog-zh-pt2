# PhotoMath 用你的相机解决数学问题

> 原文：<https://www.xda-developers.com/photomath-a-math-beginners-dream-app/>

对我来说，像这样的申请对在校学生来说非常重要。在我开始攻读大学物理学位的同一年，我买了我的第一个重要的机器人，我立刻意识到它有多么大的帮助。从精确的绘图应用程序到 TI 模拟器(不要评价我，真实的东西在这里花费惊人！)，经过 Wolfram 和 MATLAB Mobile 这样的巨头，有很多工具可以让一个人超越。事实上，我要说，如果没有 Android，我也不会选择攻读数学学位——所以谢谢你，谷歌。

对于一个机器人来说，大多数数学应用程序的问题是输入通常很麻烦或者很累。像矩阵或充满括号的长函数这样的东西，在通常只有一行的文本框中输入简直是一件痛苦的事情。尽管我的 Android 手机作为计算器有着巨大的功能，但我仍然依赖我卑微但可靠的*卡西欧 fx-570ES Plus* 来完成大多数任务——不是最好或最花哨的，但这是我在这里能负担得起的。但是，即使我在数百个出现的计算器应用程序中发现用处不大，我仍然会尝试我能找到的每一个有价值的数学应用程序，尤其是那些具有创新输入方法或良好信息输出的应用程序。

PhotoMath 两者兼而有之，但当我第一次听说它时，我有了最初的犹豫*“它可能不会工作得很好”*。用于检测现实生活中的物体或文本的应用已经取得了很大进展，我仍然记得当[世界镜头](http://questvisual.com/)让每个人都震惊的时候。PhotoMath 的问题是，它必须检测真实世界的涂鸦，然后通过识别算法传递数据，识别算法不仅仅是字母，还有数字和运算符。此外，元素的空间排列及其分布构成了被扫描内容的语法，任何函数或方程元素中的微小变化或错误都会在逻辑上破坏您想要解决的整个计算过程。在这方面，这个相机计算器应用程序非常雄心勃勃，因为它必须以绝对的精度处理一个相当粗糙的问题，才能做到它的设计目的；从一开始我就想说明**它不是为高等数学**设计的。

让我们抛开界面不谈:它太棒了。简单、直观、简洁。该应用程序比典型的材料设计应用程序更扁平，因为它缺少元素下的阴影。然而，在每一个移动的菜单中，到处都有非常好和平滑的过渡。你会发现你的输入历史在底部，帮助和反馈按钮在右边，闪光灯/提灯按钮在顶部。该中心有扫描仪，你可以用手指调整，以准确捕捉你想要的东西。没有比这更简单的了，它的直观性加上 swift 教程造就了一步到位的学习曲线。这只是工作的完美界面。

T

计算器的核心是它的功能，在这方面，应用程序是有用的，**但如果你是 STEM 学生，你可能根本不会经常打开它**。我想知道它到底能做什么，因为我听到了关于确切功能的不同评论(一些人报告说某些操作符和函数有效，而另一些人声称无效)。然而，请记住**它还不支持手写识别**。我开始使用一个长的 Sturm-Liouville 操作符 overkill，当它识别出它时，我非常非常惊讶——但是经过仔细检查，我注意到它没有接受几个符号(我会注意到这一点几次)。我慢慢发现了它的局限性，为此我必须浏览几页内容。没有线性代数(忘记变换)，没有实函数分析，没有任何形式的导数或积分，等等。就范围而言，便宜的计算器有同样的内置功能。当涉及到像解 2 级或 3 级方程这样的事情时，使用计算器算法并输入几个值可能会更快。令人惊讶的是，它确实很好地处理了不等式，包括那些带有模块的不等式。它也包括方程组和核心三角函数。

考虑到 Android 版本中仍有需要改进的地方，我认为这款应用提供了很好的服务。即使在室内，对元素的识别也出奇的准确。这是意料之中的，因为它背后的公司 Microblink 专门从事文本识别。然而，当涉及到某些特殊字符时，该应用程序有时会弄错——尤其是当它们是较小的上标或下标时。可以理解的是，与不支持的操作相关的符号也没有被删除。此外，当涉及到希腊字符时，该应用程序有点不一致。Beta (β)出现在我扫描的一些输入中，但 gamma (γ)等其他符号被混淆了(例如，与 x 混淆)。这再次表明这款应用的目标是初学数学，因为它可以接受的符号和语法与二次方程以外的运算无关。

而在这些条件下，**就是伟大的*。*** 过程![](img/5b77ccd200f2ca90faad4e1cd1714957.png) s 快，但后面的更好。该应用程序为您提供了一个非常详细的实现解决方案的步骤列表，这使得它成为那些学习如何解决方程或想要跟踪他们的错误的人的一个极好的选择。你也可以点击每一个元素来获得额外的信息，以防你不能马上知道发生了什么。在一些较长的解决方案中，过程有时在最终结果出来之前就结束了，提示您发送反馈。但是我只在不确定的方程中看到了这一点(不定相容；无限的解决方案)，所以对于大多数基本需求，这将很快满足。还有，方程组的检测非常好。与此同时，我注意到我输入的内容似乎过于关注系统的排列，在更复杂的系统中，当变量排列在一边，而不是解决方案时，它也会结束。真正有用的是，它可以为您提供简化术语的技巧，否则有些人可能不会这样做，因此它也有助于学习某些模式和优化。

 <picture>![](img/e3a41fb823d34e14176bcd8628b61847.png)</picture> 

We were just getting to the fun part..

# 结论

总而言之，这个应用程序是设计和文本识别的一个显著成就。我的手机上有很多数学应用程序解决方案，我计划在未来的社论中写下这些解决方案，虽然这不会取代我使用 Note line 的 S-pen 的 Wolfram 集成的默认方法，但对于那些不想用手写笔或笨拙的键盘写东西的人来说，这仍然是一个好主意。它让数学求解变得非常自然(同时，又不自然的不同！)，而且由于它是这种技术的首批几个值得注意的例子之一，我真的很兴奋地看到这种技术以及其他选项如何发展。现在，你会发现在实际的计算器或像 Wolfram 这样的服务中有更高的精确度和覆盖率，尽管这隐含着输入的麻烦。然而，**如果你是高中生或正在学习数学**你可能想看看这个，因为它的易用性加上强大的识别能力和信息输出使它成为一个非常方便的工具。对于那些处理多变量微积分或令人难以置信的变换的人来说，你的高端 ti 或卡西欧还没有替代品——特别是在考场上...！

***你可以在 Playstore 找到 PhotoMath [！](https://play.google.com/store/apps/details?id=com.microblink.photomath&hl=en)***

作者注:当我说这些应用程序很重要时，我并不是说我认为它们应该被广泛使用，或者它们应该取代原有课程的任何一部分。像每一种工具一样，这些应用应该被明智地使用，并受到监管。他们可能是一个相当拐杖，他们的使用，而或学习核心基础应予以劝阻。尽管如此，我看不出用它来练习你已经知道或掌握的操作有什么错。像这样的技术肯定会让学生变得懒惰，但任何一种技术如果使用不当也会变得懒惰！