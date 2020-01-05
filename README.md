OpenCore EFI
================

:exclamation: Change 'MLB', 'ROM', 'SystemSerialNumber' and 'SystemUUID' Number to a valid value!

:exclamation: This configuration is still work in progress. While it is able to boot and use most functions, not everything has been tested.

<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/UEFI/refind.png" width="640" height="360"/>

<img src="https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System/System_Info_1.png" width="698" height="465"/>

EFI Folder for OpenCore Bootloader.
Created with the help of [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)

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
| H.264           | :heavy_check_mark:       | [with Radeon RX 5700](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md#hardware-encoding)  |
| HEVC            | :heavy_check_mark:       | [with Radeon RX 5700](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md#hardware-encoding)  |
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
- [Benchmarks](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/Benchmark.md)
- [Multiboot](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/Multiboot.md)
- [Screenshots](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/System.md)
- [UEFI Settings](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/UEFI.md)
- [USB-Map](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/USB-Map.md)

### System Components

- [GIGABYTE B450 Aorus Pro Rev. 1.0](https://de.aorus.com/product-detail.php?p=794&t=53&t2=57&t3=121) (UEFI Version [F41](http://download.gigabyte.eu/FileList/BIOS/mb_bios_b450-aorus-pro_f41_n.zip))
- [AMD RYZEN 5 3600](https://www.amd.com/de/products/cpu/amd-ryzen-5-3600)
- [Crucial Ballistix Sport LT rot DIMM Kit 16GB, DDR4-3200, CL16-18-18](https://ballistixgaming.com/products/dram/sport/ballistix-sport-lt-ddr4/ballistix-sport-lt-ddr4-rc.html)
- [PowerColor Red Dragon Radeon™ RX 5700](https://www.powercolor.com/product?id=1565954303)
- [WD Blue SN500 NVMe SSD](https://shop.westerndigital.com/de-de/products/internal-drives/wd-blue-sn500-nvme-ssd#WDS500G1B0C)
- [Corsair Force Series MP510 960GB, M.2](https://www.corsair.com/de/de/Kategorien/Produkte/Datenspeicher/M-2-SSDs/Force-Series-MP510/p/CSSD-F960GBMP510)
- [Crucial MX500 500GB](http://eu.crucial.com/eur/en/ssd/storage-ssd-mx500)
- Samsung SSD 840 EVO 250GB
- [HP ENVY 27s](https://store.hp.com/GermanyStore/Merch/Product.aspx?id=Y6K73AA&opt=ABB&sel=MTO) 4K Monitor via DisplayPort
- [Fenvi FV-T919](https://www.aliexpress.com/item/4000167777406.html) WiFi / Bluetooth Card PCIe
- [Define C Tempered Glass](https://www.fractal-design.com/products/cases/define/define-c-tempered-glass/black/)

### Software Versions

- macOS Catalina 10.15.2 (19C57)
- OpenCore [0.5.3](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.5.3)

### SSDT
- SSDT-EC-AMD [Block EC Device](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/amd-config.plist/amd-config#acpi)
- SSDT-USBX-AMD [Fix USB Power](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md#fixing-usb-power-on-amd)
- SSDT-PLUG [NullCPUPowermanagement alternative patch](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/NullCPU-patch.md)

### Drivers
- ApfsDriverLoader [2.1.4](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.4)
- FwRuntimeServices [2.1.4](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.4)
- VBoxHfs [2.1.4](https://github.com/acidanthera/AppleSupportPkg/releases/tag/2.1.4)
- VirtualSMC [1.0.9](https://github.com/acidanthera/VirtualSMC/releases/tag/1.0.9)

### Tools
- UEFI Shell

### Kexts
- AGPMInjector [0.0](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/NullCPU-patch.md#3-creating-the-agpm-injector-kext)
- AppleALC Layout 1 for Realtek ALC1220-VB [1.4.4](https://github.com/acidanthera/AppleALC/releases/tag/1.4.4)
- AppleMCEReporterDisabler [1.0](https://github.com/AMD-OSX/AMD_Vanilla/blob/master/Extra/AppleMCEReporterDisabler.kext.zip)
- Custom USB Port kext [0.0](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md)
- Innie (set NVMe SSD to internal) [1.2.0](https://forums.macrumors.com/threads/innie-a-fix-for-pci-drives-seen-as-external.2136229/#post-26433989)
- Lilu [1.4.0](https://github.com/acidanthera/Lilu/releases/tag/1.4.0)
- SmallTreeIntel82576 for Intel I-211AT Ethernet [1.0.6](https://drive.google.com/file/d/0B5Txx3pb7pgcOG5lSEF2VzFySWM/view)
- VirtualSMC [1.0.9](https://github.com/acidanthera/VirtualSMC/releases/tag/1.0.9)
- WhateverGreen [1.3.5](https://github.com/acidanthera/WhateverGreen/releases/tag/1.3.5)

### Sources
- [OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
- [AMD Vanilla OpenCore](https://github.com/AMD-OSX/AMD_Vanilla/tree/opencore)
- [r/hackintosh](https://www.reddit.com/r/hackintosh/)
- [Kext Repository](https://1drv.ms/f/s!AiP7m5LaOED-m-J8-MLJGnOgAqnjGw)
- [OpenCore Bootloader](https://github.com/acidanthera/OpenCorePkg)
- [AMD-OSX Discord](https://discord.gg/EfCYAJW)
- [Wireless Buyers Guide](https://khronokernel-7.gitbook.io/wireless-buyers-guide/)
- [How to fix iMessage (tonymacx86)](https://www.tonymacx86.com/threads/how-to-fix-imessage.110471/)