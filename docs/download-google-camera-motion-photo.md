# 在 Google Pixel 上下载带有动态照片和面部修饰的 Google Camera 应用程序

> 原文：<https://www.xda-developers.com/download-google-camera-motion-photo/>

谷歌品牌的智能手机并不总是以出色的相机质量而闻名。谷歌 Nexus 智能手机系列的拍照质量一般(尽管 Nexus 6P 比其他产品略胜一筹)。直到该公司开始通过[谷歌像素系列](https://www.xda-developers.com/meet-the-new-google-pixel-and-google-pixel-xl/)采取更加以硬件为中心的重点，他们的智能手机的相机质量才会显著提高。Pixel 智能手机擅长拍照的部分原因是谷歌相机应用程序采用了谷歌的 HDR+技术。这是一个不用学习如何[编辑原始图像](https://www.xda-developers.com/the-promise-of-raw-smartphone-photography/)就能拍出漂亮照片的好方法。谷歌希望给用户更多选择来捕捉他们生活中的珍贵时刻，所以他们在谷歌相机应用程序中添加了一些新功能，包括[谷歌像素 2 和像素 2 XL](https://www.xda-developers.com/google-pixel-2-xl-announced-price/) : [运动照片、](https://www.xda-developers.com/google-pixel-2-front-facing-camera-face-retouching-motion-photo/)面部修饰和[人像模式](https://www.xda-developers.com/pixel-2-xl-stereo-speaker-music-recognition-portrait-mode/)等。

我们花了一些时间在谷歌 Pixel 2 上，并提取了一些系统 apk 供你安装。早些时候，我们发布了更新的[像素启动器](https://www.xda-developers.com/get-google-pixel-2-pixel-launcher-bottom-search-bar/) APK，它带来了新的[日历/天气小工具](https://www.xda-developers.com/google-pixel-2-calendar-widget-any-phone/)以及底部的谷歌搜索栏。现在，我们将分享最新的谷歌相机 APK，它为你现有的第一代谷歌 Pixel 和谷歌 Pixel XL 设备添加了**运动照片**和**面部修饰**。有谷歌 Nexus 设备吗？别担心，还有一些改进等着你。

动态照片是短的(~3 秒)视频剪辑，在您按下“捕捉”按钮之前和之后立即拍摄。它们不是非常高质量的视频(根据[*【Android police】*](http://www.androidpolice.com/2017/10/11/hands-motion-photos-googles-version-apples-live-photos/)，1024x768 MP4 剪辑与原始 JPEG 搭配在一起)，但它们非常擅长帮助你让你的经历更加“生动”谷歌有几张[的运动照片样本](https://photos.google.com/share/AF1QipO2_gTkgT1QwgYaWCTowaN6d2Cb5rvyJU10cjAdSU9Ao8v9Ec-r1v1cKdWEx6PNqg/photo/AF1QipP3IopzoNWtRutf8O0b0V_Tm83GIg_MdgnEWVMA?key=WEdYT3BMNFZGdUlwQ0l6aEdFT1UwVlg2LUZESDhn)供你细读。

* * *

## 在 Google Pixel/Pixel XL 上安装带有运动照片和面部修饰的 Google Camera 应用程序

要享受这一功能，您只需将下面的应用程序下载到您的手机上。我们在运行 Android 8.0 Oreo 的谷歌 Pixel XL 上测试了 APK，他们证实了动态照片确实有效！另一方面，我们的另一位测试人员表示，肖像模式和面部修饰功能不存在，但你的里程数可能会有所不同。如果这些特性最终为您所用，请大声告诉我们，我们将更新这篇文章！

[**下载支持运动照片的谷歌相机**](https://www.androidfilehost.com/?fid=745849072291680653)

不幸的是，在非谷歌设备上安装这个谷歌相机应用程序是不可能的。尽管如此，我们一直在报道的那个整洁的[非官方谷歌摄像头端口](https://www.xda-developers.com/google-camera-hdr-customization-raw-support/)为许多非谷歌设备带来了 HDR+,所以如果你渴望谷歌提供的一些最好的软件功能，你肯定会想去看看。

### 更新#1 脸部修图作品

经过多次报道，我们现在可以确认面部修饰功能确实可以在谷歌 Pixel 设备上工作。

### 更新#2 谷歌 Nexus 的改进

用户反映，这一更新极大地提高了应用程序的总体性能。比如相机取景器 FPS 增加，UI 整体更爽快。

### 更新#3 澄清“HDR+增强版”

对不起大家，但 HDR+增强版没什么特别的。谷歌只是重命名了字符串，以更好地反映 HDR+在谷歌相机应用程序中的工作方式。

```
 <string name="hdr_auto_desc">HDR+ on</string>
<string name="hdr_on_desc">HDR+ enhanced</string>
<string name="hdr_plus_auto_desc">HDR Plus on</string>
<string name="hdr_plus_on_desc">HDR Plus enhanced</string> 
```

正如你在上面的字符串中看到的，取自 APK 对最新的谷歌相机应用程序的拆卸，以前被称为 HDR+自动的现在是 HDR+ On，曾经被称为 HDR+ On 的现在是 HDR+增强。