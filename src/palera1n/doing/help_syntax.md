# palra1n的help语法

```bash
crifan@licrifandeMacBook-Pro  ~/dev/dev_tool/reverse_security/iOS/palera1n  palera1n --help
Usage: palera1n [-cCdDEfhlLnOpRsvV] [-e boot arguments] [-k Pongo image] [-o overlay file] [-r ramdisk file] [-K KPF file] [-i checkra1n file]
Copyright (C) 2023, palera1n team, All Rights Reserved.

iOS/iPadOS 15+ arm64 jailbreaking tool

    --version                Print version
    --force-revert                Remove jailbreak
    -B, --setup-partial-fakefs        Setup partial fakefs
    -c, --setup-fakefs            Setup fakefs
    -d, --demote                Demote
    -D, --dfuhelper            Exit after entering DFU
    -e, --boot-args <boot arguments>    XNU boot arguments
    -E, --enter-recovery            Enter recovery mode
    -f, --fakefs                 Boots fakefs
    -h, --help                Show this help
    -i, --override-checkra1n <file>        Override checkra1n
    -k, --override-pongo <file>        Override Pongo image
    -K, --override-kpf <file>        Override kernel patchfinder
    -l, --rootless                Boots rootless. This is the default
    -L, --jbinit-log-to-file        Make jbinit log to /cores/jbinit.log (can be read from sandbox while jailbroken)
    -n, --exit-recovery            Exit recovery mode
    -I, --device-info            Print info about the connected device
    -o, --override-overlay <file>        Override overlay
    -O, --disable-ohio            Disable Ohio
    -p, --pongo-shell            Boots to PongoOS shell
    -P, --pongo-full            Boots to a PongoOS shell with default images already uploaded
    -r, --override-ramdisk <file>        Override ramdisk
    -R, --reboot-device            Reboot connected device in normal mode
    -s, --safe-mode                Enter safe mode
    -v, --debug-logging            Enable debug logging
        This option can be repeated for extra verbosity.
    -V, --verbose-boot            Verbose boot

Environmental variables:
    TMPDIR        temporary diretory (path the built-in checkra1n will be extracted to)
```

## palera1n -I

用palera1n查看当前连接的iPhone的信息：

```bash
crifan@licrifandeMacBook-Pro  ~/dev/dev_tool/reverse_security/iOS/palera1n  palera1n -I
Mode: normal
ProductType: iPhone10,1
Architecture: arm64
Version: 15.0
DisplayName: iPhone 8 (Global)
```
