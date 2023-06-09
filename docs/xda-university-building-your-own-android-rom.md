# XDA 大学:打造自己的 Android Rom

> 原文：<https://www.xda-developers.com/xda-university-building-your-own-android-rom/>

开发并不总是感觉没有定制 rom 的开发。它们是我们移动体验中如此关键的一部分，如果不先闪现几个，就很难获得一个合适的 Android 体验。因此，如果你只是碰巧在考虑建立自己的学校，XDA 大学是开始你的旅程的好地方。

XDA 大学的《如何构建安卓只读存储器》指南是一个很好的入门概述，可以帮助您入门。虽然它实际上并没有详细说明如何实际创建进入定制只读存储器的每个组件，但它为初学者提供了基本组件的全面但可消化的分解。其中包括:

*   *内核*:“内核是每个操作系统的关键组件。它可以被视为应用程序和设备实际硬件之间的一种桥梁
*   *库*:库是专门开发来激活设备关键功能(如摄像头或扬声器)的代码块。如果你的 ROM 中没有特定的库，你的 ROM 有可能无法启动或工作。
*   *boot loader*:“boot loader 一般是机器执行的代码的第一个字节，它将告诉 bootsequence 并将操作系统加载到 RAM 中。”
*   *恢复*:恢复是一个“应用程序”，允许你刷新内核、rom、mod 和调整。这也是一种安装和更新你的 ROM，分割你的 SD 卡和许多其他操作系统相关的东西的方法。
*   *无线电*:无线电是“软件层最底层的部分”，负责“处理 GPS 天线、GSM 天线和启动 CPU:运行操作系统所需的一切”。

这些组件中的每一个对成功的 ROM 构建都很重要，如果其中一个出错，您的 ROM 可能无法启动。因此，请务必查看 XDA 大学的指南，以及 XDA 论坛中的大量指南，以获得更多指导和细节。