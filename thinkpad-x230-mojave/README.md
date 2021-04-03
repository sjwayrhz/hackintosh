# thinkpad x230 -- mac os 1.14.6

替换 EFI 到 macOS 的系统目录下即可驱动



本机使用的是 AR9285无线网卡.驱动方法如下：

- 拷贝 IO80211Family.kext 和 Kext Utility.app 到 /System/Library/Extensions 目录下
- 双击  Kext Utility.app ，依次点击下一步直到最后，大约需要3分钟
- 重启，检查无线网卡是否安装成功