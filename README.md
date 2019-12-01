OpenCore EFI
-----

<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System_Info_1.png" width="698" height="465"/>
<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System_Info_2.png" width="698" height="526"/>
<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System_Info_3.png" width="698" height="500"/>

EFI Folder for OpenCore Bootloader. Serial Number from default config.
Created with the help of [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)

## System Components

- [GIGABYTE B450 Aorus Pro Rev. 1.0](https://de.aorus.com/product-detail.php?p=794&t=53&t2=57&t3=121) (UEFI Version [F41](http://download.gigabyte.eu/FileList/BIOS/mb_bios_b450-aorus-pro_f41_n.zip))
- [AMD RYZEN 5 3600](https://www.amd.com/de/products/cpu/amd-ryzen-5-3600)
- [Crucial Ballistix Sport LT rot DIMM Kit 16GB, DDR4-3200, CL16-18-18](https://ballistixgaming.com/products/dram/sport/ballistix-sport-lt-ddr4/ballistix-sport-lt-ddr4-rc.html)
- [SAPPHIRE PULSE Radeon RX VEGA56 8G HBM2](https://www.sapphiretech.com/de-de/consumer/pulse-rx-vega56-8g-hbm2)
- [WD Blue SN500 NVMe SSD](https://shop.westerndigital.com/de-de/products/internal-drives/wd-blue-sn500-nvme-ssd#WDS500G1B0C)

## Versions

- macOS Catalina 10.15.1 (19B88)
- OpenCore 0.5.3 (30.11.2019) Commit [160556b](https://github.com/acidanthera/OpenCorePkg/commit/160556b84dc4a1225a1103d05d20181cad5f6e66)


## SSDT
- SSDT-EC-AMD

## Drivers
- ApfsDriverLoader [2.1.2](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.2)
- FwRuntimeServices [2.1.2](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.2)
- UsbKbDxe [2.1.2](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.2)
- VBoxHfs [2.1.2](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.2)
- VirtualSMC [1.0.9](https://github.com/acidanthera/VirtualSMC/releases/tag/1.0.9)

## Tools
- UEFI Shell

## Kexts
- AMD-USB-Map for GIGABYTE B450 Aorus Pro
- AppleALC Layout 7 for Realtek ALC1220-VB [1.4.3](https://github.com/acidanthera/AppleALC/releases/tag/1.4.3)
- Lilu [1.3.9](https://github.com/acidanthera/Lilu/releases/tag/1.3.9)
- NullCPUPowerManagement [1.0.0.d2](https://github.com/corpnewt/NullCPUPowerManagement)
- SmallTreeIntel82576 for Intel I-211AT Ethernet [1.0.6](https://drive.google.com/file/d/0B5Txx3pb7pgcOG5lSEF2VzFySWM/view)
- VirtualSMC [1.0.9](https://github.com/acidanthera/VirtualSMC/releases/tag/1.0.9)
- WhateverGreen [1.3.4](https://github.com/acidanthera/WhateverGreen/releases/tag/1.3.4)

## Sources
- [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [AMD Vanilla OpenCore](https://github.com/AMD-OSX/AMD_Vanilla/tree/opencore)
- [r/hackintosh](https://www.reddit.com/r/hackintosh/)
- [Kext Repository](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)
- [OpenCore Bootloader](https://github.com/acidanthera/OpenCorePkg)
