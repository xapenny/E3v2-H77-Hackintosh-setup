

# E3v2 Catalina Hackintosh

### 前言

> 前一段时间重新配了一台ivy平台的机器，平常打游戏剪视频用。这台机器黑得挺轻松的，也没有什么好介绍的。大家自取文件就行

### 注意

1. 我在config里都去掉了机器序列号和UUID，如果需要iMessage的要自己写入白苹果三码
2. 本套配置默认使用OpenCore引导，使用前需要在BIOS里修改一些项目，具体细节请参考[黑果小兵的OpenCore教程](https://blog.daliansky.net/OpenCore-BootLoader.html)

---

### 配置

|   硬件   | 描述                                                         |
| :------: | ------------------------------------------------------------ |
|   CPU    | Intel(R) Xeon(TM) E3-1230 v2 CPU @ 3.30GHz                   |
|   RAM    | 16 GB 1600 MHz DDR3                                          |
|   硬盘   | - SATA6G: Samsung SSD 860 EVO mSATA 250GB <br/>- SATA6G: UNIC S100-240 SSD 240GB<br/>- SATA3G: Seagate HDD 500GB x3 |
|   主板   | MSI ZH77a-G43                                                |
|   显卡   | AMD(R) RADEON(TM) RX 570 4GB                                 |
|   声卡   | Realtek ALC892                                               |
| 有线网卡 | 暂时用不到所以没驱动                                         |
| 无线网卡 | Broadcom BCM94360CD                                          |
|  显示器  | - DVI: Philips 193E (1440x900)                               |

---

### 工作正常

- 系统启动
- 显卡
- 无线网卡
- AppleALC声卡内建
- USB3.0
- CPU/GPU变频
- HandOff
- 个人热点
- AirDrop
- iCloud/iMessage/FaceTime (需要自己写白苹果三码)

---

### 已知问题

1. 日常使用中有几率出现冻屏，若无法接受可以将SMBIOS机型改为MacPro6,1。不会出现冻屏，代价是失去硬件解码。
3. 暂时不能睡眠，用屏幕保护代替

---

### CPU变频教程

1. 终端输入`sudo mount -uw / && killall Finder`
2. 将`IOPlatformPluginFamily.kext`放到`/系统/资源库/Extensions/`下并重建缓存
3. 重启电脑，用CPU-S可以检测到7档位变频

---

### 适用系统

- macOS 10.15 Catalina

---

### 更新日志

- 2020.1.28

> 首次发布

---

### 最后的尾巴

- 如果在使用我的文件当中出现了什么问题也欢迎来问我<xapenny@roselia.club>