# 向您的高通设备添加频段

> 原文：<https://www.xda-developers.com/add-frequency-bands-qualcomm/>

# 向您的高通设备添加频段

在特定的手机型号中，某些频段被原始设备制造商屏蔽。了解如何使用指南和计算器应用程序解锁它们。

由于运营商/原始设备制造商以及当地监管机构对频段的限制，经常出差的人无疑会拥有多台设备。从索尼、LG、三星和其他原始设备制造商那里，很容易找到几乎相同设备的地区变体。当然，这些公司希望盈利，所以他们经常出售多种设备，而不是一种可以在所有硬件支持的频段之间切换的设备。令人惊讶的是，大多数手机在没有官方支持的频段下工作得很好。事实上，这通常只是一个软件限制，可以通过 XDA 上可用的工具来规避。

多亏了两位 XDA 的资深成员，你可以尝试自己解锁一些频率: [fffft](http://forum.xda-developers.com/member.php?u=5353566) ，他发现了一种适用于三星 Galaxy S5 的方法；以及 [vndnguyen](http://forum.xda-developers.com/member.php?u=2018502) ，他开发了一个应用程序来计算高通设备所需的值。这种方法非常(明显)粗糙，但如果你想在访问其他国家时使用屏蔽的运营商，这绝对值得一试。

如果你想增加频段，你需要做好大量阅读的准备。这个过程不像简单的生根那么简单，需要一些工具，比如 QPST 和 QXDM。如果你仔细按照线索，一切顺利，你将能够在世界上任何一个国家使用这个设备。您将节省一些在当地市场上寻找设备所需的金钱和时间。当然，这样做也带有内在的风险，所以请确保在继续之前阅读并理解所有内容。

你可以通过访问这个[频段论坛线程](http://forum.xda-developers.com/galaxy-s5/general/how-to-add-rf-lte-frequency-bands-to-t2886059)来阅读 ffft 的指南。波段计算器可以在单独的[波段计算器应用线程](http://forum.xda-developers.com/android/apps-games/app-qualcomm-nv-calculator-adding-2g-3g-t2915649)中找到。