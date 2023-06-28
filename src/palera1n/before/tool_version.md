# 要清楚palera1n越狱工具的版本

* `palera1n`越狱工具的版本
  * Windows用：`palen1x`
    * 文档：
      * [Using palen1x | iOS Guide (cfw.guide)](https://ios.cfw.guide/using-palen1x/)
      * [palera1n/docs: GitBook docs for palera1n (github.com)](https://github.com/palera1n/docs)
        * [docs/flashing-palen1x.md](https://github.com/palera1n/docs/blob/main/palen1x/flashing-palen1x.md)
        * [docs/booting-palen1x.md](https://github.com/palera1n/docs/blob/main/palen1x/booting-palen1x.md)
        * [docs/jailbreak-with-palen1x.md](https://github.com/palera1n/docs/blob/main/palen1x/jailbreak-with-palen1x.md)
    * 代码仓库
      * palera1n/palen1x: Alpine-based distro that lets you install rootful and rootless palera1n-c. (github.com)
        * https://github.com/palera1n/palen1x/
  * Linux/Mac的用：`palera1n`，有2个版本
    * `shell script`
      * 旧版本是个`palera1n.sh`脚本
      * 旧版本的教程
        * [Installing palera1n (Legacy) | iOS Guide (cfw.guide)](https://ios.cfw.guide/installing-palera1n-legacy/)
          * 核心命令
            * `./palera1n.sh --tweaks 15.6.1 --semi-tethered`
    * （ 编译好的 电脑端的 直接可用的）`二进制`
      * 代码仓库
        * [palera1n/palera1n-c: palera1n written in C (github.com)](https://github.com/palera1n/palera1n-c)
          * palera1n written in C
            * 是个用C写的，在PC端（Mac、Linux等）中运行的，palera1n的二进制程序
      * 下载地址
        * [Releases · palera1n/palera1n-c (github.com)](https://github.com/palera1n/palera1n-c/releases)
          * macOS
            * palera1n-macos-universal
              * 截至20230302最新版：v2.0.0-beta.4
                * https://github.com/palera1n/palera1n-c/releases/download/v2.0.0-beta.4/palera1n-macos-universal
      * 常用参数
        * `-c`, `--setup-fakefs`       Setup fakefs
          * When used with -f, --fakefs, Create the new APFS volume required for rootful. Will fail if one already exists.
        * `-f`, `--fakefs`              Boots fakefs
          * Jailbreak in rootful mode.
        * `-l`, `--rootless`            Boots rootless. This is the default
        * `-v`, `--debug-logging`      Enable debug logging
          * This option can be repeated for extra verbosity.
        * `-V`, `--verbose-boot`       Verbose boot
      * 常见用法
        * `palera1n -cf` == `palera1n -c -f`
          * 创建fakefs
        * `palera1n -f`
          * 启动设备
        * `palera1n` == `palera1n -l` == `palera1n --rootless`
          * 无任何参数的启动，（默认）以rootless方式去越狱
            * 注意：rootless模式下支持的tweak插件很少
        * 常见用法对比
          * `palera1n -f`：`f`=`Fakefs`=`rootFul`
          * `palera1n` == `palera1n -l`：`l`=`rootLess`
      * 完整用法=语法=帮助
        * `palera1n --help`
        * 或 在线的html文档
          * palera1n - nickchan.lol
            * https://cdn.nickchan.lol/palera1n/c-rewrite/releases/v2.0.0-beta.4/palera1n.1.html
            * https://cdn.nickchan.lol/palera1n/artifacts/c-rewrite/palera1n.1.html
