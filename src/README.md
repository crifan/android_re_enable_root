# Android逆向：开启root

* 最新版本：`v2.0.0`
* 更新时间：`20241114`

## 简介

总结安卓逆向期间涉及的给安卓root。先是概览；然后是分别介绍安卓模拟器和安卓真机的root；之后详细介绍安卓真机的root的流程，包括Bootloader解锁、fastboot mode等，和涉及到的工具：TWRP、Magisk等；并且用实例去介绍如何给Android13的Pixel5去root，包括下载安装最新版Magisk、解锁Bootloader、用Magisk去给boot.img打patch、用Magisk写入patch后的boot.img和Magisk中root相关设置。以及相关知识和设备：A/B槽位、OPPO R11s的root；以及整理root相关心得。

## 源码+浏览+下载

本书的各种源码、在线浏览地址、多种格式文件下载如下：

### HonKit源码

* [crifan/android_re_enable_root: Android逆向：开启root](https://github.com/crifan/android_re_enable_root)

#### 如何使用此HonKit源码去生成发布为电子书

详见：[crifan/honkit_template: demo how to use crifan honkit template and demo](https://github.com/crifan/honkit_template)

### 在线浏览

* [Android逆向：开启root book.crifan.org](https://book.crifan.org/books/android_re_enable_root/website/)
* [Android逆向：开启root crifan.github.io](https://crifan.github.io/android_re_enable_root/website/)

### 离线下载阅读

* [Android逆向：开启root PDF](https://book.crifan.org/books/android_re_enable_root/pdf/android_re_enable_root.pdf)
* [Android逆向：开启root ePub](https://book.crifan.org/books/android_re_enable_root/epub/android_re_enable_root.epub)
* [Android逆向：开启root Mobi](https://book.crifan.org/books/android_re_enable_root/mobi/android_re_enable_root.mobi)

## 版权和用途说明

此电子书教程的全部内容，如无特别说明，均为本人原创。其中部分内容参考自网络，均已备注了出处。如发现有侵权，请通过邮箱联系我 `admin 艾特 crifan.com`，我会尽快删除。谢谢合作。

各种技术类教程，仅作为学习和研究使用。请勿用于任何非法用途。如有非法用途，均与本人无关。

## 鸣谢

感谢我的老婆**陈雪**的包容理解和悉心照料，才使得我`crifan`有更多精力去专注技术专研和整理归纳出这些电子书和技术教程，特此鸣谢。

## 其他

### 作者的其他电子书

本人`crifan`还写了其他`150+`本电子书教程，感兴趣可移步至：

[crifan/crifan_ebook_readme: Crifan的电子书的使用说明](https://github.com/crifan/crifan_ebook_readme)

### 关于作者

关于作者更多介绍，详见：

[关于CrifanLi李茂 – 在路上](https://www.crifan.org/about/)
