# palera1n越狱的前提条件

* 要满足一系列条件
  * If you want the device to be semi-tethered, you will need 5-10GB of space for the fakefs. This means that 16GB devices cannot be semi-tethered
  * If you are on A10(X), use checkp4le instead for full SEP functionality (Passcode, TouchID, Apple Pay)
  * On A11, you must disable your passcode while in the jailbroken state (on iOS 16, you need to reset your device before proceeding with palera1n A11).
  * USB-A cables are recommended to use, USB-C may have issues with palera1n and getting into DFU mode.
  * A Linux or macOS computer
    * Python 3 must be installed
    * AMD CPUs have an issue [with (likely) their USB controllers] that causes them to have a very low success rate with checkm8. It is not recommended that you use them with palera1n. If your device does not successfully jailbreak, try a computer with an Intel or other CPU
