January 2021:
- update to OpenCore 0.65 and changes in Hardware configuration.
- updated UEFI settings
- not all test have been repeated
- removed kernel boot argument "agdpmod=pikera", for usage of RX5700 this should be reapplied

OpenCore EFI
================

:exclamation: Change 'MLB', 'ROM', 'SystemSerialNumber' and 'SystemUUID' Number to a valid value!

:exclamation: This configuration is still work in progress. While it is able to boot and use most functions, not everything has been tested.

<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/UEFI/refind.png" width="640" height="360"/>

<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System/System_Info_1.png" width="698" height="465"/>

EFI Folder for OpenCore Bootloader.
Created with the help of [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)

### Function Overview

| Function        | Status                   | Comment                 |
| --------------- | :----------------------: | :---------------------- |
| AirDrop         | :heavy_check_mark:       | [with Fenvi FV-T919](https://www.aliexpress.com/item/4000167777406.html) |
| Apple Music     | :heavy_check_mark:       |                         |
| Apple TV+       | :grey_question:          |                         |
| Apple Watch unlock | :heavy_check_mark:       | [with Fenvi FV-T919](https://www.aliexpress.com/item/4000167777406.html) |
| FaceTime        | :heavy_check_mark:       | audio only, no webcam   |
| FileVault 2     | :heavy_check_mark:       |                         |
| Handoff         | :heavy_check_mark:       | [with Fenvi FV-T919](https://www.aliexpress.com/item/4000167777406.html) |
| H.264           | :heavy_check_mark:       | [with Radeon RX 5700 (outdated OpenCore + macOS)](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md#hardware-encoding-RX5700) [with Radeon RX580](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md#hardware-encoding-RX580)  |
| HEVC            | :heavy_check_mark:       | [with Radeon RX 5700  (outdated OpenCore + macOS)](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md#hardware-encoding-RX5700) [with Radeon RX580](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md#hardware-encoding-RX580)  |
| hibernate       | :heavy_multiplication_x: |                         |
| iMessage        | :heavy_check_mark:       | with valid serialnumber |
| native NVRAM    | :heavy_check_mark:       |                         |
| Netflix Safari  | :grey_question:          |                         |
| NVMe boot       | :heavy_check_mark:       |                         |
| Sidecar         | :grey_question:          |                         |
| sleep/wake      | :heavy_multiplication_x: |                         |
| UEFI boot entry | :heavy_check_mark:       | [with rEFInd](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/Multiboot.md#refind) |

### Additional Information

- [Audio Settings](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/Audio.md)
- [Multiboot](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/Multiboot.md)
- [Screenshots](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md)
- [UEFI Settings](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/UEFI.md)
- [USB-Map](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/USB-Map.md)

### System Components

- [GIGABYTE B450 Aorus Pro Rev. 1.0](https://www.gigabyte.com/Motherboard/B450-AORUS-PRO-rev-10) (UEFI Version [F60e](https://download.gigabyte.com/FileList/BIOS/mb_bios_b450-aorus-pro_f60e.zip))
- ~~[AMD RYZEN 5 3600](https://www.amd.com/de/products/cpu/amd-ryzen-5-3600)~~ -> [AMD RYZEN 3 3300X](https://www.amd.com/de/products/cpu/amd-ryzen-3-3300x)
- [Crucial Ballistix Sport LT rot DIMM Kit 16GB, DDR4-3200, CL16-18-18](https://ballistixgaming.com/products/dram/sport/ballistix-sport-lt-ddr4/ballistix-sport-lt-ddr4-rc.html)
- ~~[PowerColor Red Dragon Radeon™ RX 5700](https://www.powercolor.com/product?id=1565954303)~~ -> [ASUS Dual Radeon RX 580 OC](https://www.asus.com/Motherboards-Components/Graphics-Cards/All-series/DUAL-RX580-O8G/)
- [WD Blue SN500 NVMe SSD](https://shop.westerndigital.com/de-de/products/internal-drives/wd-blue-sn500-nvme-ssd#WDS500G1B0C)
- ~~[Corsair Force Series MP510 960GB, M.2](https://www.corsair.com/de/de/Kategorien/Produkte/Datenspeicher/M-2-SSDs/Force-Series-MP510/p/CSSD-F960GBMP510)~~ -> [Kingston A2000 NVMe PCIe SSD 1TB](https://www.kingston.com/germany/en/ssd/a2000-nvme-pcie-ssd)
- ~~[Crucial MX500 500GB](http://eu.crucial.com/eur/en/ssd/storage-ssd-mx500)~~
- ~~Samsung SSD 840 EVO 250GB~~
- [HP ENVY 27s](https://store.hp.com/GermanyStore/Merch/Product.aspx?id=Y6K73AA&opt=ABB&sel=MTO) 60Hz 4K Monitor via HDMI
- [AOC 24G2U/BK](https://eu.aoc.com/en/gaming-monitors/24g2u-bk) 144Hz 1080p Monitor via HDMI
- [Fenvi FV-T919](https://www.aliexpress.com/item/4000167777406.html) WiFi / Bluetooth Card PCIe
- [Define C Tempered Glass](https://www.fractal-design.com/products/cases/define/define-c-tempered-glass/black/)

### Software Versions

- macOS Catalina 10.15.7 (19H114)
- OpenCore [0.6.5](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.6.5)

### SSDT
- SSDT-EC-USBX-DESKTOP [AMD EC+USBX SSDT](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml)

### Drivers
- OpenRuntime [0.6.5](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.6.5)
- HfsPlus [x.x.x](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)

### Tools
- UEFI OpenShell

### Kexts
- ~~AGPMInjector [0.0](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/NullCPU-patch.md#3-creating-the-agpm-injector-kext)~~
- AppleALC Layout 1 for Realtek ALC1220-VB [1.5.6](https://github.com/acidanthera/AppleALC/releases/tag/1.5.6)
- AppleMCEReporterDisabler [1.2](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
- Custom USB Port kext [0.0](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md)
- ~~Innie (set NVMe SSD to internal) [1.2.0](https://forums.macrumors.com/threads/innie-a-fix-for-pci-drives-seen-as-external.2136229/#post-26433989)~~
- Lilu [1.5.0](https://github.com/acidanthera/Lilu/releases/tag/1.5.0)
- NVMeFix [1.0.5](https://github.com/acidanthera/NVMeFix/releases/tag/1.0.5)
- SmallTreeIntel82576 for Intel I-211AT Ethernet [1.3.0](https://github.com/khronokernel/SmallTree-I211-AT-patch/releases/tag/1.3.0)
- VirtualSMC [1.1.9](https://github.com/acidanthera/VirtualSMC/releases/tag/1.1.9)
- WhateverGreen [1.4.6](https://github.com/acidanthera/WhateverGreen/releases/tag/1.4.6)

### Sources
- [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [AMD Vanilla OpenCore](https://github.com/AMD-OSX/AMD_Vanilla/tree/opencore)
- [r/hackintosh](https://www.reddit.com/r/hackintosh/)
- ~~[Kext Repository](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)~~
- [OpenCore Bootloader](https://github.com/acidanthera/OpenCorePkg)
- [AMD-OSX Discord](https://discord.gg/EfCYAJW)
- [Wireless Buyers Guide](https://khronokernel-7.gitbook.io/wireless-buyers-guide/)
- [How to fix iMessage (tonymacx86)](https://www.tonymacx86.com/threads/how-to-fix-imessage.110471/)