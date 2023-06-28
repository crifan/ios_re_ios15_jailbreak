# palera1n越狱后的常见问题

## 缺少常用解压缩工具

现象：palera1n越狱后，没有自动安装常用的解压缩工具(插件)，即zip unzip gzip unrar p7zip bzip2等等，需要自己去安装

解决办法：

有2种方式：

* 手动找到对应的deb地址，并下载得到deb文件，自己手动用dpkg安装
  * 去哪里找deb地址？
    * 去这里：
      * https://www.ios-repo-updates.com
    * 贴出部分deb地址
      * zip
        * http://tigisoftware.com/rootless/debs/zip_3.0_iphoneos-arm.deb
      * unzip
        * https://apt.procurs.us/pool/main/iphoneos-arm64/1700/unzip/unzip_6.0-27_iphoneos-arm.deb
      * gzip
        * https://apt.procurs.us/pool/main/iphoneos-arm64/1700/gzip/gzip_1.12_iphoneos-arm.deb
      * unrar
        * https://apt.procurs.us/pool/main/iphoneos-arm64/1700/unrar_6.1.4_iphoneos-arm.deb
      * p7zip
        * https://repo.chimera.sh/debs/p7zip_16.02_iphoneos-arm.deb
      * bzip2
        * https://apt.procurs.us/pool/main/iphoneos-arm64/1700/bzip2_1.0.8_iphoneos-arm.deb
  * 如何安装？
    * 去iPhone中安装
      * Mac通过ssh登录iPhone，或进入iPhone中的终端
    * 安装命令
      * dpkg -i xxx.deb
* Sileo中，找到对应的软件源，添加软件源，搜索对应插件，去安装
  * （包含这些解压缩工具的）软件源的地址：
    * https://apt.procurs.us
