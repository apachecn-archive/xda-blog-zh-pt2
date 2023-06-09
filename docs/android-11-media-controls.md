# Android 11 的媒体控件最多可以记忆 5 次之前的媒体会话

> 原文：<https://www.xda-developers.com/android-11-media-controls/>

今天早些时候，谷歌为新的 Android 11 测试版发布了大量新视频和开发者文档。虽然我们已经在以前的文章中记录了许多新特性和 API，但 Google 在新发布的文档中总会透露一些信息。其中一个最新功能被称为“媒体控制”，实际上这是一个比谷歌最初在 Android 11 测试版公告中透露的功能有趣得多的功能。

但首先，让我们回顾一下 Android 11 中新的媒体控制功能的作用。在 Android 5.0 Lollipop (API level 21)中，Google 引入了一种通知类型，叫做“ [MediaStyle](https://developer.android.com/reference/android/app/Notification.MediaStyle) ”这种通知样式用于媒体播放通知，在扩展形式中支持多达 5 个操作，显示一个通常包含专辑插图等内容的大图标。大多数流媒体应用程序的开发人员实现了这种通知风格，但问题是有大量的流媒体应用程序可以显示自己的媒体播放通知。

谷歌现在正在整合媒体播放通知，在 Android 11 的快速设置面板中为媒体播放器创建一个专用的持久空间。这使用户可以轻松访问媒体控制，无论显示的是什么应用程序，或者还有什么其他通知等待处理。媒体控制也可以显示在锁定屏幕上。此外，谷歌在右上角增加了一个新按钮，可以启动输出选择器对话框，用户可以快速选择他们想要在什么设备上播放他们的媒体。

也许新的媒体控制功能最好的部分是媒体播放通知现在可以在媒体播放会话或设备重新启动时保持不变。如果一个应用程序实现了 [MediaBrowserService](https://developer.android.com/reference/android/service/media/MediaBrowserService) 和 [MediaSession](https://developer.android.com/reference/android/media/session/MediaSession) ，那么 SystemUI 可以在快速设置面板/锁定屏幕的媒体控制部分显示多达 5 个之前的会话。

如果有多个媒体会话可用，Android 11 会将它们安排在一个可移动的转盘中。轮播按顺序列出媒体会话，从电话上本地播放的流到远程流(如 cast 会话),再到以前的可恢复会话(按上次播放的顺序)。

这意味着，如果你最近结束了 Spotify、Pandora、YouTube Music 或其他流媒体应用程序中的媒体会话，这意味着它们的媒体播放通知不再可见，你不必再次打开这些应用程序来恢复播放。

在 Android 11 Beta 1 中，目前默认不启用该功能。用户必须进入设置>开发者选项，然后切换“媒体恢复”来显示新的媒体控件。请注意，谷歌在其官方 Android 11 公告[中分享的截图来自比 Beta 1](https://twitter.com/dsandler/status/1270794251182497792) 稍新的版本，但功能仍然存在，因此谷歌鼓励媒体应用程序的开发者尝试这一新功能。

有关新媒体控件如何工作的更多信息，请查看[谷歌的开发者文档](https://developer.android.com/preview/features/media-controls)或观看下面来自 SystemUI 团队的 Dan Sandler 的视频(时间标记为 7:30)。