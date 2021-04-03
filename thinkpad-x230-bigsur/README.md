# EFI -- xxx

EFI参考链接如下

```
https://github.com/dungnt11/thinkpad-x230
```

AR9285无线网卡驱动如下：

```
https://www.asly.top/archives/188
```

无线网卡驱动方法：

- 安装并打开 opencore configuration，
- 点击macos最上层状态栏的opencore configuration图标按钮，可以挂在EFI目录 ，打开/Volumes/EFI/EFI/OC/Kexts。
- 拷贝 AirPortAtheros40.kext 和 HS80211Family.kext到/Volumes/EFI/EFI/OC/Kexts目录下。
- 使用OpenCore Configurator打开 /Volumes/EFI/EFI/OC/Config.plist
- 选择 Kernel , 将 HS80211Family.kext拷贝到WhateverGreen.kext下
- 将 AirPortAtheros40.kext拷贝到HS80211Family.kext下
- 修改config→Misc→Security→SecureBootModel为disabled
- 重启，检查无线网卡驱动成功。

