# 对 Galaxy S II 进行重新分区，以获得更多应用或媒体存储空间

> 原文：<https://www.xda-developers.com/repartition-your-galaxy-s-ii-for-more-app-or-media-storage/>

不管你怎么说[*/数据/媒体*设备](http://www.xda-developers.com/android/what-is-a-data-media-device/)固有的不便，但它们也有它们的优点。虽然 USB 大容量存储模式通常被认为对直接磁盘操作更加用户友好，对于大量数据传输更加可靠，但 MTP 设备允许单个*/数据*分区来处理媒体和应用程序存储。将媒体和应用程序存储都放在一个分区内意味着您永远不会用完应用程序存储空间，同时在您的内部 SD 卡上有许多可用空间。

像三星 Galaxy S II 这样的老设备通常使用单独的挂载点来存储应用程序和媒体。对于那些安装了不成比例的大量应用程序或大量媒体的人来说，这可能会导致存储空间问题。在他的 SGS2 上遇到问题后，XDA 的高级成员 [metalgearhathaway](http://forum.xda-developers.com/member.php?u=2069027) 决定通过重新分区他的内部存储来解决问题，以牺牲媒体存储来释放额外的应用存储空间。他不仅自己解决了问题，还在论坛上分享了解决方案。

该补丁以各种包含新分区信息的 PIT 文件的形式出现，可以通过 Odin 应用。有几种不同的 PIT 文件可用，允许您根据自己的需要定制存储细分。例如，如果你有很多应用程序，但不需要太多的媒体存储，你可以为应用程序分配多达 12g 的空间。另一方面，如果你没有太多的应用程序，而希望有尽可能多的媒体空间，那么你可以只为应用程序投入 1g 的空间。

自然，任何再分配都会带来巨大的内在风险。此外，您显然会丢失设备上存储的所有数据。然而，如果你正确地遵循这些步骤，回报可能是值得冒险和争论的。转到[原始线程](http://forum.xda-developers.com/showthread.php?t=2538947)开始。