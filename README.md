# [OpenCore](https://github.com/acidanthera/OpenCorePkg) configuration for Ryzen 3700X &amp; MSI B450I Gaming Plus AC

## Builds

| Type                   | Name                                  |
| ---------------------- | ------------------------------------- |
| CPU                    | Ryzen 3700X                           |
| MB                     | MSI B450I Gaming Plus AC              |
| Audio                  | ALC887                                |
| GPU                    | RX 6800 XT (All Polaris & Navi cards) |
| RAM                    | 16G DDR4 (8G * 2)                     |
| Wireless & Bluetooth   | DW1820A                               |
| macOS                  | Big Sur & Catalina                    |

## Read Me First!

- This config adopts the RX 6800 XT and
  it's [Smart Access Memory](https://www.amd.com/en/technologies/smart-access-memory)
  by default, you need to enable `Resizeable Bar` and `Above 4g memory` properties in BIOS.
- If your cpu don't have 8 cores (e.g. 6 core 5600X), you must change patch values
  of `algrey - Force cpuid_cores_per_package` to boot your system.
  See [AMD_Vanilla ReadMe](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first) for details.

## Functional

- [x] CPU by [AMD-Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
- [x] USB
  by [khronokernel's guide](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md)
- [x] Audio by [AppleALC](https://github.com/acidanthera/AppleALC) (alcid=5)
- [x] Graphics by [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [x] WIFI by [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) (brcmfx-country=#a)
- [x] Bluetooth by [BrcmPatchRAM](https://github.com/RehabMan/OS-X-BrcmPatchRAM)
  and [nickhx from osxlatitude](https://osxlatitude.com/forums/topic/11540-dw1820a-the-general-troubleshooting-thread/page/10/)
- [x] iMessage / FaceTime / Airdrop / Handoff

## Issues

- mic in of alc887 don't work
- Can't run andriod emulator since android emulator only supports vt-x, but genymotion and virtualbox with amd-v support
  work well
