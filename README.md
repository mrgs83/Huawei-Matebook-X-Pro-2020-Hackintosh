# Huawei Matebook X Pro 2020 macOS Catalina 10.15.05
 OpenCore Config to run macOS Catalina on the Matebook X Pro 2020


| Device  | Spec |
| ------------- | ------------- |
| CPU  | Intel i5-10210U Comet Lake  |
| IGPU  | Intel UHD 620 / Comet Lake GT2 |
| GPU  | Nvidia MX250 (disabled)  |
| Audio Codec  | ALC256 (Possible ID's: 17,19,57,76,97)  |
| WIFI  | Intel AC9560  |
| Trackpad  | I2C HID Based  |
| Touchscreen  | I2C HID Based  |
| SSD  | 512GB WDC PC SN730  |

What's working:
- Battery Status (Patched DSDT)
- iGPU Acceleration
- Brightness Keys (Patched DSDT)
- CPU Power Management

Semi working:
- Bluetooth using [OpenIntelWireless](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)(Can connect for a short time)

Not working:
- Trackpad and Touchscreen (Hotpatch required)
- Audio (New Layout-ID required)
- WIFI (Should be possible with [itlwm](https://github.com/OpenIntelWireless/itlwm/blob/master/.github/README_en.md))


# Installation:
Use the included Clover folder on a USB Drive to install macOS Catalina on the Laptop. Credits to [Laozhiang](https://github.com/laozhiang/MateBook_13_14_XPro-Hackintosh)

# Post Installation:
Replace the Clover folder on your USB Drive with the OpenCore Folder from my repo. This folder will be updated each time I make improvements.
Boot into macOS, mount your internal and external EFI volumes and copy over OpenCore to your internal SSD.
