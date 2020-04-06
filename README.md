# EFI for Ryzen 3700X &amp; MSI B450I Gaming Plus AC

## Builds

| Type                   | Name                                  |
| ---------------------- | ------------------------------------- |
| CPU                    | Ryzen 3700X                           |
| MB                     | MSI B450I Gaming Plus AC              |
| Audio                  | ALC887                                |
| GPU                    | XFX Radeon RX 5700 8 GB               |
| RAM                    | 16G DDR4 (8G * 2)                     |
| Wireless & Bluetooth   | DW1820A                               |
| macOS                  | 10.15.x (OpenCore) / 10.15.1 (Clover) |

## BIOS Setting
- [Above 4G memory] Enabled

## Functional

- [x] CPU by [AMD-Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
- [x] USB by [khronokernel's guide](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md)
- [x] Audio by [AppleALC](https://github.com/acidanthera/AppleALC) (alcid=5)
- [x] Graphics by [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [x] WIFI by [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) (brcmfx-country=#a)
- [x] Bluetooth by [BrcmPatchRAM](https://github.com/RehabMan/OS-X-BrcmPatchRAM) and [nickhx from osxlatitude](https://osxlatitude.com/forums/topic/11540-dw1820a-the-general-troubleshooting-thread/page/10/)
- [x] iMessage / FaceTime / Airdrop / Handoff

## Issues

- mic in of alc887 don't work
- Can't run andriod emulator since android emulator only supports vt-x, but genymotion and virtualbox with amd-v support work well
