# AutoVoice 集成终于进入了 Google Home，下面是它的使用方法

> 原文：<https://www.xda-developers.com/autovoice-integration-finally-makes-its-way-to-google-home-heres-how-to-use-it/>

在谷歌的批准悬而未决一个月后，AutoVoice 终于被批准用作谷歌 Home 的第三方集成。与 AutoVoice 集成，您可以发送命令到您的手机，Tasker 将能够作出反应，让您执行无数的自动化脚本直接从您的声音。

以前，这需要一个复杂的解决方案，涉及 IFTTT 通过 Join 向你的设备发送命令，但现在你可以直接向你的设备发送自然语言命令。我们在 XDA 一直在[等待这个版本](https://www.xda-developers.com/unlocking-the-true-power-of-google-home-with-autovoice/)，现在它在这里，我们将向你展示如何使用它。

* * *

## Google Home 的真正力量已经被释放

上面的视频是由 AutoVoice 的开发者若奥·迪亚斯在 AutoVoice 集成获得批准之前制作的。我在这里重新链接它只是为了展示这种集成的可能性，这是我们现在都可以享受的东西，因为谷歌终于推出了对每个人的自动语音支持。与任何 Tasker 插件一样，这需要一点学习曲线，所以尽管集成从昨晚就开始了，但许多人仍然不知道如何让它工作。我从昨晚就开始玩这个了，我将向你展示如何通过与 Google Home 对话来触发你自己的 AutoVoice 命令。

来自 AutoVoice 开发者若奥·迪亚斯的请求:请注意，今天是 AutoVoice 与 Google Home 整合并对所有用户开放的第一天。因此，可能有一些错误还没有被消除。请放心，在 AutoVoice/Home 集成发布到 Play Store 中 AutoVoice 的稳定频道之前，他正在努力修复他遇到的任何东西。

* * *

## 入门指南

在利用这种新的集成之前，您需要具备一些条件。第一个，也是最明显的要求，就是你需要一个 Google Home 设备。如果你还没有，可以在谷歌商店和其他零售商那里买到。亚马逊 Alexa 支持也正在等待批准，所以如果你有其中之一，你必须等待，然后才能尝试这种集成。

一旦安装了这些应用程序，就该开始工作了。你需要做的第一件事是在 Google Home 应用中启用 AutoVoice 集成。打开 Google Home 应用程序，然后点击右上角的遥控器/电视图标。这将打开“设备”页面，其中列出了您当前连接的启用 cast 的设备(包括您的 Google Home)。点击三点菜单图标，打开谷歌主页的设置页面。在“谷歌助手设置”下，点击“更多”最后，在列出的 Google Home 集成部分下，点击“服务”,调出可用的第三方服务列表。向下滚动，在列表中找到“AutoVoice ”,在集成的“关于”页面中，您将找到启用集成的链接。

一旦您启用了这种集成，您现在就可以通过您的 Google Home 与 AutoVoice 对话了！通过说“**好的谷歌，让自动语音打招呼”**或“**好的谷歌，让我和自动语音说话”来检查它是否被启用**如果你的 Google Home 回复“当然，这里有 AutoVoice”，然后进入 auto voice 命令提示符，那么集成正在工作。现在我们可以设置 AutoVoice 来识别我们的命令。

* * *

## 设置自动语音

出于本教程的考虑，我们将制作一个简单的 Tasker 脚本来帮助您定位您的手机。通过说出“查找我的手机”的任何自然变化，Tasker 将开始播放一个响亮的哔哔声，这样你就可以快速辨别你把你的设备放在哪里了。当然，你可以通过 GPS 定位你的设备，然后给自己发送一封附有相机拍摄的照片的电子邮件，从而轻松地使这变得更加复杂，但我们将重点关注的部分只是教你如何让 Tasker 识别你的 Google Home 语音命令。使用你的声音，有两种方法可以通过 Google Home 向 Tasker 发出命令。

第一种是按照你设置的指令说出你的指令**。这意味着**在你的指挥中绝对没有犯错的余地。例如，如果你想定位你的设备，并且你设置 Tasker 识别你说的“查找我的手机”，那么你**必须准确地对你的 Google Home 说**“查找我的手机”(不要有任何其他单词插入或放在开头或结尾)，否则 Tasker 将无法识别该命令。解决这个问题的唯一方法是想出尽可能多的可能的命令变体，例如“查找我的设备”、“定位我的电话”、“定位我的设备”，并希望您记得说出您设置的命令的至少一个变体。换句话说，第一种方法遇到了与通过 IFTTT 设置 Tasker 集成完全相同的问题:**它对于您的语言来说非常不灵活。******

第二种，也是我喜欢的方法，是使用自然语言。自然语言命令允许您自然地对设备说话，Tasker 仍然能够识别您在说什么。例如，如果我说一些更长的话，如“好的，谷歌，你能让自动语音尽快找到我的设备吗？”它仍然会识别我的命令，即使我在我的口头命令中加入了多余的“请”和“尽快”。得益于 API 的强大功能，这一切都成为可能。AI，这是 AutoVoice 检查你的语音命令的依据，以解释你想说的话，并返回你可能设置的任何变量。

听起来很棒！你可能和我一样，对第二种选择更感兴趣。不幸的是，自然语言命令对 Dias 先生的服务器来说负担很重，所以你需要**注册每月 0.99 美元的订阅服务**才能使用自然语言命令。这是一个有点令人沮丧的要求，但考虑到它的成本有多低，它将使你的谷歌之家变得多么强大和有用，这个费用是非常公平的。

重要提示:如果你想对你的 Google Home 设备说出“自然语言命令”，那么你需要遵循以下步骤。否则，跳到下面的创建命令。

* * *

## 设置自然语言命令

由于 AutoVoice 依赖于 API。对于人工智能的自然语言处理，我们需要建立一个 API。AI 账号。[进入网站](https://api.ai/)点击“免费注册”进行免费注册。在开发控制台中，创建一个新的代理，并将其命名为 **AutoVoice** 。将代理**设为私有**，点击**保存**即可创建代理。保存代理后，它将出现在主 API 下的左侧栏中。AI logo。

一旦你创建了你的 API。AI 帐户，您将需要获得您的访问令牌，以便 AutoVoice 可以连接到您的帐户。单击新创建的代理旁边的齿轮图标，显示 AutoVoice 代理的设置页面。

在“API 密匙”下，你会看到你的**客户端访问令牌**和你的**开发者访问令牌。**你将**需要保存两个**。在您的设备上，打开 AutoVoice 测试版。点击“自然语言”打开设置页面，然后点击“设置自然语言”现在，在给定的文本框中输入两个令牌。

现在，AutoVoice 将能够从 API.AI 发送和接收命令。但是，在您订阅 AutoVoice 之前，此功能会受到限制。回到自然语言设置页面，点击“命令”现在，除了一个名为“默认回退意图”的命令外，命令列表应该是空的(注意在我的截图中，我已经自己设置了几个)。在底部，你会注意到一个名为“**的开关，用于谷歌助手/Alexa。**"如果您启用此开关，系统会提示您订阅 AutoVoice。如果您希望使用自然语言命令，请接受订阅。

* * *

## 创建 Tasker 配置文件以响应自然语言命令

打开 Tasker，点击右下角的“+”按钮，创建一个新的配置文件。单击“事件”创建新的事件上下文。事件上下文是一个触发器，只在上下文被识别时触发一次——在这种情况下，我们将创建一个链接到 AutoVoice 自然语言命令的事件。在事件类别中，浏览至插件->自动语音->自然语言。

点击铅笔图标进入配置页面，创建 AutoVoice 自然语言命令。点击“**创建新命令**来创建自动语音命令。在向您展示的对话框中，您会看到一个文本输入位置来输入您的命令，以及另一个文本输入位置来输入您希望 Google Home 说的响应。键入或说出您想要 AutoVoice 识别的命令。虽然不要求您列出希望它识别的命令的所有可能的变体，但至少要列出一些以防万一。

* * *

**提示**:你可以通过长按其中一个单词来创建输入命令的变量。在弹出的窗口中，你会看到一个“**创建变量**选项，旁边是通常的剪切/复制/选择/粘贴选项。如果您选择此项，您将能够将这个特定的单词作为变量传递给 API。AI，它可以通过 API.AI 返回。当您希望 Google Home 以可变响应进行响应时，这可能会很有用。

例如，如果您构建了一个命令“play songs by $artist ”,那么您可以让响应返回变量中设置的艺术家的姓名。因此，你可以在同一个命令下说“播放缪斯的歌曲”或“播放电台司令的歌曲”，你的 Google Home 会以你在命令中提到的相同乐队/艺术家名称做出响应。我下面的教程没有使用这个特性，因为它是为更高级的用例保留的。

* * *

构建完命令后，单击 finished。您将会看到一个弹出的对话框，询问您想为自然语言命令命名什么。给它起个描述性的名字。默认情况下，它以您输入的第一个命令命名该命令，这就足够了。

接下来，它会问你要设置什么动作。这允许您自定义发送到设备的命令，该命令将存储在 **%avaction 中。**例如，如果您将操作设置为“findmydevice**”**文本“find my device”将存储在%avaction 变量中。这对我们的教程没有任何作用，但是在后面的教程中，我们会用到更高级的命令。

单击顶部的复选标记退出命令创建屏幕，因为您现在已经完成了自然语言命令的构建和保存。现在，我们将创建一个任务，当自然语言命令被识别时，该任务将被触发。当你回到 Tasker 的主屏幕，你会看到“新任务”创建弹出窗口。单击“新建任务”创建一个新任务。单击“+”图标将您的第一个操作添加到此任务中。在音频下，点击**媒体音量**将**级别设置为 15** 。返回到任务编辑屏幕，您将在列表中看到您的第一个操作。现在创建另一个动作，但这一次点击“**警报”**并选择“**嘟嘟声”**将**持续时间**设置为**10000 ms**并将**振幅**设置为 **100%。**

如果你做的正确，你应该在任务列表中有下面两个动作。

退出任务创建屏幕，您就**完成了。**现在您可以测试您的创作了！简单地说“**好的，谷歌，让自动语音找到我的手机”**或任何想到的自然变化，你的手机应该开始大声蜂鸣 10 秒钟。你唯一需要说的是让 Google Home 启动 AutoVoice 的触发器——“好的，Google，问 auto voice”或“好的，Google，让我和 auto voice 说话”部分。之后说的任何话，都可以随心所欲的自由流动，自然，API 的魔力。人工智能使你可以灵活地使用你的语言！

一旦你开始创建大量的自然语言命令，从 Tasker 编辑它们可能会很麻烦。幸运的是，你可以直接从 AutoVoice 应用程序中编辑它们。打开 AutoVoice，点击“自然语言”调出其设置。在 Commands 下，您现在应该看到我们刚刚创建的自然语言命令！如果你点击它，你几乎可以编辑命令的每一个方面(甚至设置变量)。

* * *

## 创建 Tasker 配置文件以响应非自然语言命令

如果您不想订阅 AutoVoice，您仍然可以创建一个类似于上面的命令，但它要求您列出您能想到的触发该任务的所有可能的短语组合。这种设置的最大不同在于，当您创建事件上下文时，您必须选择自动语音识别的而不是自动语音自然语言。您将以类似的方式构建您的命令列表和响应，但是 API。人工智能不会处理任何部分解析你的口头命令，所以你必须 100%准确地说出这些短语之一。当然，您仍然可以像使用自然语言一样编辑这些命令。

否则，构建链接的任务与上面相同。唯一不同的是任务是如何触发的。有了自然语言，你可以说得更自如。如果没有自然语言，你必须非常小心你的命令。

* * *

## 结论

我希望你现在明白如何将 AutoVoice 与 Google Home 集成。对于任何 Tasker 新手来说，绕过 Tasker 学习曲线仍然是一个问题。但是如果你有使用 Tasker 的经验，这篇教程应该是你创建自己的 Google Home 命令的一个很好的起点。或者，您可以在此处以[视频形式查看 Dias 先生的教程。](https://www.youtube.com/watch?v=q21X3wVAXI8)

在我使用 Google Home 的有限时间里，我已经想出了十几个相当有用的创意。在未来的文章中，我将向你展示如何制作一些非常酷的 Google Home 命令，例如通过语音打开/关闭 PS4、阅读所有通知、阅读你的最后一条短信等等。我不会破坏我已有的东西，但我希望这篇教程能让你对即将到来的事情感到兴奋！