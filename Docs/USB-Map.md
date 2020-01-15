USB Map
================

![back](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/USB-Map/IO_Shield.png)![front](https://github.com/mipxx/OpenCoreEFI/blob/master/Docs/USB-Map/Mainboard.png)


two USB Controllers
- PTXH
- XHC0

| Portnumber      | USB 3.0 Name (Address), Controller   | USB 2.0 Name (Address), Controller  | Comment |
| :-------------: | :---------------: | :---------------: | ------- |
| 1               | PRT7 (0x07), XHC0 | PRT3 (0x03), XHC0 |         |
| 2               | PRT5 (0x05), XHC0 | PRT1 (0x01), XHC0 |         |
| 3               | POT1 (0x01), PTXH | POT5 (0x05), PTXH |         |
| 4               | POT2 (0x02), PTXH | POT6 (0x06), PTXH |         |
| 5               | PRT6 (0x06), XHC0 | PRT2 (0x02), XHC0 |         |
| 6               | PRT8 (0x08), XHC0 | PRT4 (0x04), XHC0 |         |
| 7a              | - | PO11 (0x0B), PTXH | Fenvi FV-T919 Bluetooth |
| 7b              | - | PO12 (0x0C), PTXH | unused |
| 8a              | - | PO13 (0x0D), PTXH | unused |
| 8b              | - | PO14 (0x0E), PTXH | unused |
| 9a              | POT4 (0x04), PTXH | POT8 (0x08), PTXH | Fractal Define C Front left |
| 9b              | POT3 (0x03), PTXH | POT7 (0x07), PTXH | Fractal Define C Front right |
