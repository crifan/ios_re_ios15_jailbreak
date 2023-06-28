# palera1n

* palera1n
  * 资料
    * 主页
      * https://palera.in/
        * palera1n is a developer-oriented jailbreak for checkm8 devices (A8-A11) on iOS 15.0-16.3
    * github
      * https://github.com/palera1n/
        * https://github.com/palera1n/palera1n
  * 前提条件
    * checkm8 vulnerable iOS device
  * 支持的iOS版本：`iOS/iPadOS 15+`
    * iOS 15.x or 16.x
      * iOS 15.0 ~ iOS 16.3.1
  * 支持的iOS设备
    * 芯片类型/架构：`arm64`
      * `A11`及之前
        * 注：`A12+`（架构是`arm64e`）就不支持了
    * 机型
      * iPhone 6s Plus
      * iPhone SE (2016)
      * iPhone 7
      * iPhone 7 Plus
      * iPhone 8
      * iPhone 8 Plus
      * iPhone X
      * 
      * iPad mini 4
      * iPad Air 2
      * iPad (5th generation)
      * iPad (6th generation)
      * iPad (7th generation)
      * iPad Pro (9.7")
      * iPad Pro (12.9") (1st generation)
      * iPad Pro (10.5")
      * iPad Pro (12.9") (2nd generation)
      * 
      * iPod Touch (7th generation)
  * 支持2种越狱模式/越狱类型
    * `rootful` = `fakefs-rootful` = `普通越狱` = `有根越狱`：rootfs可写，包括根目录/也可以写
    * `rootless` = `无根越狱`：rootfs只读，只有/var可写
  * 推荐的越狱模式
    * rootful越狱=有根越狱=普通越狱
      * 这样对于之前的兼容性会更好
      * 很多插件等，应该可以正常工作了
      * 比如希望的`frida`等等
