# iOS逆向：iOS15越狱

* 最新版本：`v1.2.1`
* 更新时间：`20240318`

## 简介

介绍iOS越狱中的iOS 15+之后的越狱工具和事项。包括palera1n、XinaA15、Dopamine等。先是iOS15+的越狱概览，然后是北背景知识，包括rootless和rootful、iPhone机型信息、免签安装ipa文件；以及详细介绍iPhone中安装TrollStore；接着介绍palera1n，包括越狱前的前提条件、注意事项和说明、工具的版本、文档和资料，和越狱中的palera1n的rootful越狱概述和详解，以及常见问题、help语法、loader app和越狱后的ssh、如何恢复越狱、常见问题；接着介绍XinaA15，包括越狱前的历史版本和下载地址，和越狱中的安装XinaA15、用XinaA15越狱，以及越狱后的界面和功能；接着介绍Dopamine；最后给出参考资料。

## 源码+浏览+下载

本书的各种源码、在线浏览地址、多种格式文件下载如下：

### HonKit源码

* [crifan/ios_re_ios15_jailbreak: iOS逆向：iOS15越狱](https://github.com/crifan/ios_re_ios15_jailbreak)

#### 如何使用此HonKit源码去生成发布为电子书

详见：[crifan/honkit_template: demo how to use crifan honkit template and demo](https://github.com/crifan/honkit_template)

### 在线浏览

* [iOS逆向：iOS15越狱 book.crifan.org](https://book.crifan.org/books/ios_re_ios15_jailbreak/website/)
* [iOS逆向：iOS15越狱 crifan.github.io](https://crifan.github.io/ios_re_ios15_jailbreak/website/)

### 离线下载阅读

* [iOS逆向：iOS15越狱 PDF](https://book.crifan.org/books/ios_re_ios15_jailbreak/pdf/ios_re_ios15_jailbreak.pdf)
* [iOS逆向：iOS15越狱 ePub](https://book.crifan.org/books/ios_re_ios15_jailbreak/epub/ios_re_ios15_jailbreak.epub)
* [iOS逆向：iOS15越狱 Mobi](https://book.crifan.org/books/ios_re_ios15_jailbreak/mobi/ios_re_ios15_jailbreak.mobi)

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
