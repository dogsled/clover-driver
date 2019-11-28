# Hackintosh-Install
[TOC]

## 本项目归纳黑苹果安装过程
## 工具
### 1.[clover](https://github.com/CloverHackyColor/CloverBootloader/releases)
### 2.[Clover Configurator](https://mackie100projects.altervista.org/download-clover-configurator/)
### 3.[hackintool.zip](http://headsoft.com.au/download/mac/Hackintool.zip)

## 驱动

### x. SMC [VirtualSMC](https://github.com/acidanthera/VirtualSMC/releases) 暂时待定
### x. SMC [fakeSMC](https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/) 历史可用
### x. 基础patch包 [Lilu](https://github.com/acidanthera/Lilu/releases)
### x. patch扩展 [LiluFriend](https://github.com/PMheart/LiluFriend/releases)
### x. 显示辅助[WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases)
### x. USB驱动 [RehabMan-USBInjectAll-2018-1108.zip](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/)
### x. 网卡驱动 [RTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)
### x. 声卡驱动 [AppleALC](https://github.com/acidanthera/AppleALC/releases)
### x. 变频驱动[CPUFriend](https://github.com/acidanthera/CPUFriend/releases)
    ResourceConverter.sh (https://github.com/acidanthera/CPUFriend/blob/master/Tools/ResourceConverter.sh)
    粗鲁使用教程（https://blog.daliansky.net/CPUFriend-Installation-and-Usage.html）
    变频教程（https://change-y.github.io/2018/04/30/%E5%88%A9%E7%94%A8CPUFriend-kext%E5%AE%9E%E7%8E%B0%E5%8F%98%E9%A2%91/）
### x. ps2键盘鼠标[VoodooPS2Controller](https://github.com/acidanthera/VoodooPS2/releases)
### x. 同步多核心时钟频率 [VoodooTSCSync](https://github.com/RehabMan/VoodooTSCSync)
    [https://bitbucket.org/RehabMan/VoodooTSCSync/downloads/](https://bitbucket.org/RehabMan/VoodooTSCSync/downloads/)

    此驱动必须安装 不安装会出现： still waiting for root device 错误
### x. 睡眠修复[HibernationFixup](https://github.com/acidanthera/HibernationFixup/releases)
### x. 欺骗pciid驱动 [FakePCIID](https://bitbucket.org/RehabMan/os-x-fake-pci-id/downloads/)


## 制作U盘启动盘

        官方地址[https://support.apple.com/zh-cn/HT201372](https://support.apple.com/zh-cn/HT201372)
- 下载固件
- 制作启动盘  
macOS Sierra 10.12.X 的示例:
```
sudo /Applications/Install\ macOS\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume --applicationpath /Applications/Install\ macOS\ Sierra.app
```
- 安装引导 clover
 ![image](images/WX20191127-101515.png)
- 配置config.plist文件
