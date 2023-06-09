# 谷歌展示了其在环境计算隐藏界面方面的工作

> 原文：<https://www.xda-developers.com/google-showcases-hidden-interfaces-ambient-computing/>

为了创造与周围环境无缝融合的设备，谷歌正在开发隐藏界面，除非在使用中，否则这些界面是不可见的。该公司此举背后的想法是*“创造环境计算设备和电器，可以保持日常材料的美感，同时提供按需访问交互和数字显示。”*在最近的一篇博客文章中，谷歌研究展示了其在环境计算的隐藏界面方面的工作，并强调了用于创建高亮度、低成本显示器的创新技术，这些显示器可以从纺织品、木皮、丙烯酸或单向镜子等材料下面出现。

谷歌指出，AMOLED 显示屏对于环境计算设备来说并不理想，因为它们制造起来过于昂贵和复杂。低成本的液晶显示器和电子墨水显示器也不合适，因为它们“没有足够的亮度穿透材料。”因此，该公司决定采用无源矩阵有机发光二极管(PMOLEDs)，这种器件为*提供了“一种可以显著降低成本和复杂性的简单设计”*然而，该公司指出，PMOLEDs 通常使用扫描线渲染，*“有源驱动电路一次顺序激活一行，这一过程会限制显示器亮度并引入闪烁。”*

为了克服这个问题，谷歌提出了一种使用并行渲染而不是扫描线渲染的系统，增加了亮度，减少了闪烁。利用这一解决方案，谷歌开发了概念验证隐藏接口，该接口使用 128x96 分辨率的 PMOLED 显示器，将所有行和列驱动器路由到一个连接器，以便直接访问。我们使用带有 14 个 16 通道数模转换器(DAC)的定制印刷电路板(PCB ),直接与来自 Raspberry Pi 3 A+的 224 条线路接口。触摸交互是通过围绕显示器的环形 PCB 实现的，该 PCB 具有 12 个呈弧形排列的电极。”

由此产生的隐藏界面原型展示了日常材料下的明亮和富有表现力的渲染，如所附 GIF 所示。虽然这些界面比谷歌目前在其 [Nest Audio](https://www.xda-developers.com/google-nest-audio-review/) 智能扬声器上使用的隐藏指示器大了一步，但它们仍然显示基本信息。谷歌现在计划添加图像和复杂的矢量图形，并创造高效的硬件设计。关于这项技术的更多细节，请点击下面的链接查看原始博文。

值得一提的是，这些隐藏的交互界面仍处于原型阶段，你不应该期望很快在谷歌产品上看到它们。

* * *

**来源:** [谷歌 AI 博客](https://ai.googleblog.com/2022/04/hidden-interfaces-for-ambient-computing.html)