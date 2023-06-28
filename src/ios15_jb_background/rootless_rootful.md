# rootful普通越狱 vs rootless无根越狱

* 概述
  * `rootful`越狱=普通越狱=**有根**越狱
    * rootfs可写，包括根目录/也可以写
      * palera1n中也叫：`fakefs-rootful`
  * `rootless`越狱 = **无根**越狱
    * rootfs只读，只有/var可写
* 详解
  * 之前的`普通越狱`=`成熟越狱`=`有根越狱` vs `无根越狱`=`rootless jailbreak`
    * 之前的`普通越狱`=`成熟越狱`=`有根越狱`：`iOS 15`之前
      * 越狱工具（有机会利用系统漏洞实现）：对于iOS的根文件系统`rootfs`，去读写
        * 重新挂载根文件系统（为读写）
    * `无根越狱`=`rootless jailbreak`：`iOS 15`之后
      * iOS
        * 内部机制增加了：（Apple的）`SSV`=`Signed System Volume`
          * 细节：对于原本的，被iOS设计为只读readonly的各种系统目录
            * 如果尝试去写入，则会由于filter过滤 和 nullifying而被拒绝 -》即，不允许写入
        * 效果：不允许对于rootfs去写 == `sealed ROOT File System`
      * 越狱工具
        * 无法改动/写入iOS的根文件系统`rootfs`
        * 想要实现越狱，则只能：避免写入=改动iOS 15的`rootfs`
        * 所以：新的iOS 15之后的越狱工具，都是 `rootless jailbreak`=`无根越狱`
          * rootless=对于rootfs没有写入的权限=没法改动rootfs根文件系统
          * 特殊
            * 不过有2个特殊的目录，可以写入：
              * `/var`
              * `/private/preboot`
            * 而新的iOS 15之后的越狱系统，基本上都是利用这个机制，去实现越狱的效果
              * 即：把越狱相关工具和内容，都放到`/var`（和`/private/preboot`）中
        * 说明
          * rootless jailbreak，并不表示没有root用户=root user
            * 你还是可以以`root user`身份去操作：SSH连接到设备，修改（`/var`和`/private/preboot`）中的文件的
          * 由此使得，取消越狱=卸载越狱=恢复原始设备，就变得很容易
            * 因为只是涉及到`/var`和`/private/preboot`，不涉及到整个rootfs的改动和恢复，所以很快很方便
          * 相对来说：绕过越狱检测，相对容易一些
            * 估计指的是，只是针对`/var`，而不是整个系统，所以简单点？
      * rootless有哪些影响
        * **部分插件**`tweak`失效
          * 之前的各种(依赖于旧的rootfs存放文件的)插件tweak：就失效了
            * 需要tweak插件作者去更新，才能支持新的`rootless jailbreak`
        * `bootstrap`也失效了
          * bootstrap：用于启动阶段，安装各种Unix工具，包管理器等等
          * 现在需要用改用：兼容rootless的bootstrap = rootless (compatible) bootstrap
            * 比如
              * `Procursus`
                * 【整理】iOS越狱相关：Procursus
              * `Elucubratus`
        * 文件管理器filesystem browsers：`Filza`, `SSH`, and `Apple File Conduit`
          * 基本可用：只是无法write修改系统目录中文件了（可以读取read和执行execute）
            * 可以写入`/var`和`/private/preboot`目录
