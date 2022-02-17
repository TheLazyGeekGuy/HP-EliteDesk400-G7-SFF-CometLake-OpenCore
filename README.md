# DEBUG
# HP EliteDesk400 G7 SFF CometLake Opencore 
## Catalina - Opencore 0.7.7


| Bootloader & Version     ||
|----       |---|
|SmBios     | 	iMac20,1|
|BootLoader | 	[OpenCore 0.7.7](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html) |



## [Specs](https://support.hp.com/us-en/document/c06713398)

| Component      | Brand                                     |
|----------------|-------------------------------------------|
| **CPU**        | `Intel i5 10500`(1)                                                                    |
| **Chipset**    | [`Intel Q470`]() |
| **iGPU**       | `Intel iGPU UHD 630` (8086-9BC8 / 103C-8719 Rev 03)       |
| **Storage**    | `Internal nmve Samsung PM991 250GB` [(unsupported)](https://dortania.github.io/Anti-Hackintosh-Buyers-Guide/Storage.html)                     |
| **Audio**      | `Realtek ALC3205` (ALC222[^1])[ Revision / layout (OC "layout-id") : 0x100001, layout 11](https://github.com/acidanthera/AppleALC/wiki/Supported-codecs)              |
| **Ethernet**   | `Intel I219LM`                            |
| **Wifi / BT**   | `Intel Wi-Fi 6 AX201 NGW` [kext : OpenIntelWireless](https://github.com/OpenIntelWireless/itlwm/releases/tag/v2.1.0)                            |
| **Expansion Card**   | none |
|    |  HP FLEX IO v2 Option Cards expansions :  |
|    |  - [USB Type C 3.1 Gen2 10 Gbps ](https://www8.hp.com/h20195/v2/GetPDF.aspx/c06712909.pdf) (HP 13L59AA)  |
|    |  - [USB Type C 3.1 Gen2 Port with 100W](https://www8.hp.com/h20195/v2/GetPDF.aspx/c06712909.pdf) (HP 13L60AA)) |
| **OS**         | `macOS Catalina`          |
| **BIOS**       | `2.39`                    |

[^1]: [see more](https://github.com/CLAY-BIOS/Lenovo-ThinkPad-T450s-Hackintosh-OpenCore/blob/master/EFI/OC/Kexts/AppleALC.kext/Contents/Info.plist)


### [BIOS Settings](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#intel-bios-settings)


### [Keyboard Layout Detail](https://github.com/acidanthera/OpenCorePkg/blob/master/Utilities/AppleKeyboardLayouts/AppleKeyboardLayouts.txt) 


|Key 	          |Type     |	Value   |
|----           |---      |---      |
|prev-lang:kbd 	|String 	|en-US:0  |
|prev-lang:kbd 	|String 	|fr:1     |



### What works :

- [x] Intel HD 630 iGPU HDMI 
- [x] Intel HD 630 iGPU eDP 
- [x] HDMI Audio
- [x] Intel I219LM Network
- [x] Internal Speakers
- [x] Internal headphones
- [x] Internal Output
- [x] All USB3 Ports 
- [x] All USB2 Ports 
- [x] SpeedStep / Sleep / Wake  (Fixes [[0](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html#preparations)] [[1](https://www.tonymacx86.com/threads/the-cause-of-sleep-wake-issues-with-hd530-hd630.295700/page-2)])
- [x] Wi-Fi  
- [x] Bluetooth Native
- [ ] SSD NVME Slot-1 PCIe Gen3x4
- [x] NVRAM (Native)
- [x] RTC Clock
