# 如何在 Snapseed 中选择自定义图像大小调整限制

> 原文：<https://www.xda-developers.com/how-to-select-a-custom-image-resizing-limit-in-snapseed/>

Snapseed 是谷歌子公司 Nik Software 开发的一款应用。该应用程序用于在你的设备上编辑照片，包括处理原始相机文件，这是它最大的吸引力之一。您可以编辑 RAW。通过曝光、高光、阴影、对比度、结构、饱和度、温度和色调生成 dng 文件。您还可以在共享/导出照片之前调整图像大小。这是我的相机拍的一张照片，旁边是用 RAW 拍摄并在 Snapseed 中冲洗的同一张照片。

无论你是否喜欢添加到第二个图像的变化，在保持相同的整体质量的同时，图片会有很大的差异，这要归功于 RAW 处理。

然而，Snapseed 不仅用于处理原始文件。它还用于应用滤镜、裁剪照片和调整照片大小，尽管有一些限制。在 Snapseed 中调整图像大小时，您会受到它们提供的图像宽度选项的限制。您可以调整图像的最大宽度为 4000 像素，然后纵横比保持不变以计算高度。这意味着对于任何大于 4000 像素宽的文件，你不能将它们的大小调整到 4000 以上。比如 OnePlus 3，4640x3480 的拍摄。如果我想将图像的大小调整为 4500x3375(保持 4:3 的宽高比)，那么我不能在 Snapseed 中这样做。但是，可以通过修改位于 Snapseed 的数据文件夹中的文件来增加此限制。要编辑这个文件，你需要一个支持 root 的文件探索应用，比如我们的应用&游戏论坛的免费 [MiXplorer](https://forum.xda-developers.com/showthread.php?t=1523691) ！然而，任何其他根支持的文件浏览器应该工作正常。本教程也可能对任何想将图像调整到不可用的宽度(如 1000 像素)的人有用。

[appbox xda com.mixplorer]

对于本教程，您将需要使用 Magisk 或 SuperSU 的 root 访问权限。您还需要任何根启用文件资源管理器。这不能保证在 Snapseed 的未来版本中有效。**这不能用于放大图像**。

* * *

## 自定义 snapseed 图像大小调整

确保您的设备是根设备，并且您有一个启用了根设备的文件资源管理器。如果你做到了，你就可以走了！

### 第一步

首先，您应该在文件资源管理器中导航到**/data/data/com . Nik software . snapseed/shared _ prefs/**文件夹。****

我们要编辑的文件是**com . Nik software . snapseed _ preferences . XML**。继续在你的文本编辑器中打开它！

### 第二步

查找字符串“**pref _ export _ setting _ long _ edge**”。它应该看起来像下面这样。

如您所见，我将该值更改为 4500。这意味着我的图像如果我选择调整大小，宽度将调整到 4500 像素。

请注意，在实际的调整图像大小设置中，Snapseed 会将图像大小调整值视为“null”。这没问题，因为它仍然使用我们定义的值。

* * *

## 结果呢

可以看到，我们的修改工作完美！图像成功地调整了大小，并保持了元数据的完整性。

* * *

## 说明

很明显，Snapseed 只是读取首选项文件，并直接从中进行操作。通过“图像大小”类别说“空”，我们知道应用程序不知道如何显示我们输入的值。尽管我们添加的只是一个数字，但 Snapseed 似乎只能显示它支持的正确值。尽管如此，当在 Snapseed 中执行图像大小调整时，它仍然根据首选项文件中的值正确处理图像，因此我们可以使用我们想要的任何值，只要我们选择的数字是整数。