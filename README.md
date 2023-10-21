# XPS-9360-macOS

## Kexts

**Main Kexts**
| Kext                | Version |
| ------------------- | ------- |
| AirportBrcmFixup    | 2.1.7   |
| AppleALC            | 1.8.5   |
| Lilu                | 1.6.7   |
| VirtualSMC          | 1.3.2   |
| VoodooI2C           | 2.8.0   |
| VoodooI2CHID        | 2.8.0   |
| VoodooPS2Controller | 2.3.5   |
| WhateverGreen       | 1.6.6   |

**Bluetooth Kexts**
| Kext             | Version |
| ---------------- | ------- |
| BlueToolFixup    | 2.1.7   |
| BrcmFirmwareData | 2.1.7   |
| BrcmPatchRAM3    | 2.6.8   |

**Enhanched Functions Kexts**
| Kext                  | Version |
| --------------------- | ------- |
| BrightnessKeys        | 1.0.3   |
| CPUFriend             | 1.2.7   |
| CPUFriendDataProvider | 1.2.7   |
| ECEnabler             | 1.0.4   |
| FeatureUnlock         | 1.1.5   |
| HibernationFixup      | 1.4.9   |
| NVMefix               | 1.1.1   |
| RealtekCardReader     | 2.1.0   |
| SMCBatteryManager     | 1.3.2   |
| SMCLightSensor        | 1.3.2   |
| SMCProcessor          | 1.3.2   |
| SMCSuperIO            | 1.3.2   |
| USBToolBox            | 1.1.0   |
| UTBMap                | 1.1.0   |


## BIOS Settings
When you first boot to the bootloader, follow these steps:

1. Press the `space` key to enter the modGRUBShell.
2. Type the following commands:

```bash
setup_var 0x4de 0x00  # Disable CFG Lock
setup_var 0x785 0x06  # Increase DVMT pre-allocated size to 192M For FHD version, it's also recommended setting to 192M
setup_var 0x786 0x03  # Increase CFG Memory to maximum
```