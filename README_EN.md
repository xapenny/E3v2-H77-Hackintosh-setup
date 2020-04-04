

# E3v2 Catalina Hackintosh

- English
- [简体中文](https://github.com/xapenny/E3v2-Catalina-Hackintosh-setup/blob/master/README.md)

### Opening

> I built this Ivy Bridge setup early 2020 for scripting and video editing. Hackintoshing this setup is pretty simple, here's something you need to boot macOS Catalina using OpenCore boot loader. 

### Notice

1. I removed the UUID,MLB,ROM and Serial Number. You have to generate a new one with Clover Configurator, or you will not able to boot your device
2. I use OpenCore as my bootloader. You have to change your BIOS settings first, check the list below.

| Enable               | Disable                              |
| -------------------- | ------------------------------------ |
| VT-x                 | Fast Boot                            |
| Above 4G decoding    | CFG Lock (MSR 0xE2 write protection) |
| Hyper Threading      | VT-d                                 |
| Execute Disable Bit  | CSM Support                          |
| EHCI/XHCI Hand-off   |                                      |
| OS type: other types |                                      |

---

### Hardware Configuration

|     硬件      | 描述                                                         |
| :-----------: | ------------------------------------------------------------ |
|      CPU      | Intel(R) Xeon(TM) E3-1230 v2 CPU @ 3.30GHz                   |
|      RAM      | 16 GB 1600 MHz DDR3                                          |
|  Hard Drive   | - SATA6G: Samsung SSD 860 EVO mSATA 250GB <br/>- SATA6G: UNIC S100-240 SSD 240GB<br/>- SATA3G: Seagate HDD 500GB x3 |
|  Motherboard  | MSI ZH77a-G43                                                |
| Graphics Card | AMD(R) RADEON(TM) RX 570 4GB                                 |
|  Audio Card   | Realtek ALC892                                               |
|   Ethernet    | Realtek RTL8111E PCI Express Gigabit Ethernet                |
| WiFi/BT Card  | Broadcom BCM94360CD                                          |
|    Monitor    | Philips 193E (1440x900)                                      |

---

### Working

- System Booting
- Graphics
- Apple Watch Unlock 
- H.264 + H.265 + HEVC Hardware video decoding
- CD/DVD/BD burning
- Blu-ray Disk
- Wifi/Bluetooth
- AppleALC Audio card built-in
- USB3.0 + Customise USB ports
- CPU/GPU Frequency scaling
- HandOff
- Personal Hotspot
- AirDrop
- iCloud/iMessage/FaceTime (You have to set a proper serial number to get this working)

---

### Known Issue

3. Apple Watch Unlock will failed after wake up from sleep/hibernation, I'm working on a fix.

---

### Target OS Version

- macOS 10.15 Catalina

---

### Changelog

- 2020.4.4

> 1.Changed OpenCore to another fork。
> 2.Add booting Windows without applying anything from OC's kexts/DSDTs/vendor spoof. So you can now get OEM drivers/software(like Lenovo UltraNav and FN shortcuts) work on Windows boot with OpenCore.
> 3.Add background(1440x900) for the Picker. Ps: You have to ensure that your display resolution equals \EFI\OC\Icons\background.png, or it won't show up. If you're using 4K display, do the same thing to background4k.jpg

- 2020.3.23
> 1.Update OpenCore to 0.5.7 beta
> 2.Add GUI
> 3.Fixed frozen

- 2020.2.5

> 1. Update Config.plist
> 2. Fixed ethernet
> 3. Update OpenCore to 0.5.5


- 2020.1.28

> Initial Release

---

### Support

- If there is any problem, you can leave an issue or mail me at <xapenny@roselia.club>
