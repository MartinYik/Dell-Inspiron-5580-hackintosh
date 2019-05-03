# DELL-inspiron-5580安装 MacOS Mojave

## 电脑配置

------

| 规格     | 详细信息                                                     |
| -------- | ------------------------------------------------------------ |
| 电脑型号 | DELL-inspiron-5580                                           |
| 处理器   | Intel(R) Core(TM) i5-8265u CPU @ 1.60Ghz                     |
| 内存     | 8GB  DDR4 2400MHz                                            |
| 硬盘     | BC501 NVMe SK hynix(128G/固态硬盘) <br>ST1000LM035-1RK172(1T/机械硬盘) |
| 集成显卡 | Intel Graphics UHD 620  <br>Nvidia GeForce MX150(屏蔽)       |
| 声卡     | Realtek ALC236(layout-id:47 尚未提交)                        |
| 网卡     | 英特尔 Wireless-AC 9462(无解)，使用USB无线网卡               |

## 已知问题：

------

- 读卡器（应该无解）。  
- 英特尔网卡（目前全球无解）。  

## 正常功能：

------

- 显卡  
- 声卡  (注入id：47)
- hdmi输出  
- 网卡(使用usb网卡) 
- 触摸板正常，手势全部可用。  
- usb全部正常。  
- 电池电量显示正常。  
- 摄像头正常使用 
- 睡眠正常,支持fn+insert键睡眠。  
- 变频正常。  
- 支持原生亮度快捷键。  
- 触摸板手势支持拖移锁定。

## 安装中遇到的问题

------

- 安装原版完成后，提示未能完成安装。不用管他直接点重启即可（Restart），其实已经安装成功。目前原因未知，我有一次安装遇到这个问题
- 安装好后无法使用触摸板，或者升级后触控板无法使用。你需要在每次更新系统后重建缓存。运行 `Kext Utility.app` 或者在 `终端.app` 输入 `sudo kextcache -i /`，然后重启。  
- 耳机插上没有声音。请安装[ALCPlugFix]([https://github.com/MartinYik/Dell-Inspiron-5580-hackintosh/blob/master/ALCPlugFix/install%E5%8F%8C%E5%87%BB%E8%87%AA%E5%8A%A8%E5%AE%89%E8%A3%85.command](https://github.com/MartinYik/Dell-Inspiron-5580-hackintosh/blob/master/ALCPlugFix/install双击自动安装.command))守护进程

## 更新日志

- 2019年5月5日
  - 初版efi，目前基本完美

## 特别鸣谢

- **@宪武**大神制作的众多hotpatchu补丁
- **[张丑丑](<https://github.com/daggeryu>)**大神提供的[dell-5488的clover](<https://github.com/daggeryu/DELL-inspiron-5488>)进行参考

## 致谢

- [RehabMan](https://github.com/RehabMan) 提供的   [VoodooPS2Controller](https://github.com/RehabMan/OS-X-Voodoo-PS2-Controller)等驱动。    
- [vit9696](https://github.com/vit9696) 提供的 [Lilu](https://github.com/acidanthera/Lilu) ， [AppleALC](https://github.com/acidanthera/AppleALC) ， [WhateverGreen](https://github.com/acidanthera/WhateverGreen)。     
- [Alexandred](https://github.com/alexandred)及其开发团队提供的[VoodooI2C](https://github.com/alexandred/VoodooI2C) 驱动。  
