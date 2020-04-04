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

## Functional

- [x] CPU by [AMD-Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
- [x] USB by [XLNC's script](https://forum.amd-osx.com/viewtopic.php?f=24&t=4986)
- [x] Audio by [AppleALC](https://github.com/acidanthera/AppleALC) (alcid=7)
- [x] Graphics by [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [x] WIFI by [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) (brcmfx-country=#a)
- [x] Bluetooth by [BrcmPatchRAM](https://github.com/RehabMan/OS-X-BrcmPatchRAM) and [nickhx from osxlatitude](https://osxlatitude.com/forums/topic/11540-dw1820a-the-general-troubleshooting-thread/page/10/)
- [x] iMessage / FaceTime / Airdrop / Handoff

## Issues

- Unknown processor in About This Mac (need to modify system files)
- Wrong ram speed display in About This Mac (shows half speed)
- No 32-bit support
- Can't run andriod emulator since android emulator only supports vt-x, but genymotion and virtualbox with amd-v support work well
