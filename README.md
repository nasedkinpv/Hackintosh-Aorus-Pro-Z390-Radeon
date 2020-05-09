# Hackintosh Gigabyte Z390 Aorus Pro/Intel 9th Generation/Radeon
## macOS Catalina 10.15.4
### OpenCore 0.5.8
- Motherboard — Gigabyte Aorus Pro Z390
- Processor — Intel Core i9 9900K (8 cores / 16 threads, Coffee Lake)
- Memory — Kingston HyperX Fury DDR4 (2x16GB 3066 MHz)
- SSD — Samsung NVMe EVO Pro 512GB
- Wi-Fi — TP-Link Archer T9E
- GPU — Sapphire Radeon RX 480 (new ones will work too)

[[OpenCore — Coffee Lake Guide](https://dortania.github.io/OpenCore-Desktop-Guide/config.plist/coffee-lake.html)]

[[OpenCore — Intel HD 630](https://dortania.github.io/OpenCore-Desktop-Guide/extras/gpu-patches.html)]

[[OpenCore — NVRAM B360, B365, H310, H370, Z390 Chipset](https://dortania.github.io/hackintosh/updates/2020/01/20/nvram.html)]

[[OpenCore — Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)]

## What working
- Native Power Management
- APFS
- Wi-FI — AirportBrcmFixup.kext
- Ethernet — IntelMausi.kext
- Audio — AppleALC.kext
- GPU/iGPU Hardware Acceleration — WhateverGreen / RadeonBoost
- USB and internal USB-C — from [[sarkrui build]([https://github.com/sarkrui/Hackintosh-Z390-Aorus-Pro-9700K-RX580])]
- iCloud Services / Handoff
- DRM Content
- HEVC/H264 encoding with FFmpeg
### Known issues
—

## Guide
### BIOS Setup
* Update your bios to latest F12d — [[download link](https://download.gigabyte.com/FileList/BIOS/mb_bios_z390-aorus-pro_f12d.zip)]
### Generate your SMBIOS
* GenSMBios [[GitHub link](https://github.com/corpnewt/GenSMBIOS)]
For reference, follow this guide [[OpenCore — Fix iServices](https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html)]
Platform name — iMac19,1.
### Correct your config.plist
HINT: ROM — you can use your ethernet MAC address
![N|Solid](http://nasedk.in/public/hackintosh_smbios.png)
### UEFI Drivers
![N|Solid](http://nasedk.in/public/hackintosh_uefi_drivers.png)
### Kexts
![Z390 Aorus Pro Kexts](http://nasedk.in/public/hackintosh_kexts.png)

## Overview



### GeekBench 5
![N|Solid](http://nasedk.in/public/hackintosh_geekbench.png)
![N|Solid](http://nasedk.in/public/hackintosh_metal.png)
### HEVC/H264 Intel UHD 630 Hardware Acceleration
![N|Solid](http://nasedk.in/public/hackintosh_hardware_acceleration.png)

### Credits
| Author | Link |
| ------ | ------ |
| Apple | [https://apple.com] |
| OpenCore Bootloader | [https://github.com/acidanthera/OpenCorePkg] |
| sarkrui | [https://github.com/sarkrui/Hackintosh-Z390-Aorus-Pro-9700K-RX580] |
| cmer | [https://github.com/cmer/gigabyte-z390-aorus-master-hackintosh] |
