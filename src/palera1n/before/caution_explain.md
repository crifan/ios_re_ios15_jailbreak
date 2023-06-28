# palera1n越狱的注意事项和说明

* 注意事项和说明
  * palera1n jailbreaks any iOS/iPadOS device with an arm64 (arm64e excluded) on iOS 15+, utilizing the checkm8 bootROM exploit.
    * 不支持A11之后的arm64e
      * 注：我之前的iPhone11，就是A12芯片，就是arm64e，所以不支持
  * arm64e devices will NEVER be supported.
    * 永远不会支持arm64e
  * palera1n is able to jailbreak the device in fakefs-rootful mode, where / is writable, as well as rootless mode, where / cannot be written to.
    * palera1n支持：
      * fakefs-rootful = rootful=伪造根文件系统 越狱：根目录/可写入
      * rootless=无根越狱：根目录/不可写入
  * Due to the nature of the checkm8 exploit, palera1n is semi-tethered. That is, you must run the palera1n tool after the device reboot in order to enter the jailbroken state. However, it is not required for the device to boot.
    * 是非完美越狱：
      * 原因：checkm8决定的
        * 结果：每次重启（iPhone）后，要重新运行palera1n（去恢复越狱）
          * 注：启动boot时不需要
  * On A11 devices, that is, iPhone 8, iPhone 8 Plus and iPhone X, the passcode cannot be used.
    * A11设备（iPhone8、iPhone 8P、iPhoneX）中，不能用passcode
  * On iOS 15, the passcode must be off while jailbroken.
    * iOS 15中必须关闭passcode（才能越狱）
  * On iOS 16, the passcode must be off since restore, and Reset All Contents and Settings from settings app counts as a restore. A backup may be used in this case.
    * iOS 16中，passcode必须关闭，且如果之前开启过passcode，则需要恢复出厂设置=重置系统
