

# E3v2 Catalina Hackintosh

- [English](https://github.com/xapenny/E3v2-Catalina-Hackintosh-setup/blob/master/README_EN.md)
- 简体中文

### 前言

> 前一段时间重新配了一台ivy平台的机器，平常打游戏剪视频用。这台机器黑得挺轻松的，也没有什么好介绍的。大家自取文件就行

### 注意

1. 我在config里都去掉了机器序列号、MLB、ROM和UUID，如果需要iMessage的要自己写入白苹果三码
2. 本套配置默认使用OpenCore引导，使用前需要在BIOS里修改一些项目，具体细节请参考[黑果小兵的OpenCore教程](https://blog.daliansky.net/OpenCore-BootLoader.html)

---

### 配置

|   硬件   | 描述                                                         |
| :------: | ------------------------------------------------------------ |
|   CPU    | 英特尔(R) Xeon(TM) E3-1230 v2 CPU @ 3.30GHz                   |
|   RAM    | 16 GB 1600 MHz DDR3                                          |
|   硬盘   | - SATA6G: 三星 SSD 860 EVO mSATA 250GB <br/>- SATA6G: 紫光 S100-240 SSD 240GB<br/>- SATA3G: 希捷 HDD 500GB x3 |
|   主板   | 微星 ZH77a-G43 (H77芯片组)                                                |
|   显卡   | AMD(R) RADEON(TM) RX 570 4GB                                 |
|   声卡   | 瑞昱 ALC892                                               |
| 有线网卡 | 瑞昱 RTL8111E 千兆以太网                |
| 无线网卡 | 博通 BCM94360CD 二合一卡                                         |
|  显示器  | 飞利浦 193E (1440x900)                                      |

---

### 工作正常

- 系统启动
- 显卡
- Apple Watch解锁
- H.264+HEVC硬解码(可看DRM)
- DVD/BD刻录
- 蓝光光盘播放
- 无线网卡
- AppleALC声卡内建
- USB3.0+端口定制
- CPU/GPU变频
- HandOff
- 个人热点
- AirDrop
- iCloud/iMessage/FaceTime (需要自己写白苹果三码)

---

### 已知问题

1. 睡眠唤醒后不能用Apple Watch解锁

---


### 适用系统

- macOS 10.15 Catalina

---

### 更新日志
- 2020.8.7
> 1. 更新支持11.0 macOS Big Sur
> 2. 旧版本文件已经存档供Catalina用户使用，Catalina分支不再做更新。

- 2020.4.20

> 1. 更新OpenCore版本到0.5.8
> 2. 更新驱动版本至最新

- 2020.4.4

> 1. 切换OC分支
> 2. 添加Windows引导（OC不会再对Windows作出任何修改，可以正常使用OEM驱动软件，比如TP的热键驱动）
> 3. 添加引导界面壁纸(1440x900)，请自行修改位于/EFI/OC/Icons下的background.png(或background4k.png，取决于你的显示器分辨率)

- 2020.3.23
> 1. 更新OpenCore版本到最新0.5.7
> 2. 增加GUI
> 3. 彻底解决冻屏

- 2020.2.5

> 1. 更新Config.plist
> 2. 驱动有线网卡
> 3. 更新OpenCore至0.5.5
> 4. Tools增加最新版OCC，支持OpenCore v0.5.7


- 2020.1.28

> 首次发布

---

### 最后的尾巴

- 如果在使用我的文件当中出现了什么问题也欢迎来问我<xapenny@roselia.club>
