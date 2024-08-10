# ideapad-gaming-3-ryzen5-5500h_OpenCoreEFI

### Abstract
Latest OpenCore EFI specifically and only for this laptop.

### Supported Devices
> - **Lenovo Ideapad Gaming 3 (The version with Ryzen 5500H and RTX 2050)**
### MacOs supported versions
> - MacOs `13.6.8 ` Ventura \
Any earlier version will propably work too. I haven't tested with Sonoma yet. 
### IMPORTANT:
**Because you have to use the iGPU built in the Ryzen CPU, I highly recommend to disable the RTX 2050 in UEFI firmware settings. \
I haven't been able to boot macOS Ventura. After disabling RTX 2050, It has booted successfully! \
You can do that by selecting UMA Graphics instead of Switchable graphics. \
And also you should assign maximum VRAM to iGPU (2GB), also in the UEFI firmware settings. (UMA Frame Buffer Size)**

## Laptop Configuration

| Hardware    | Additional Information                                                         |
| ----------- | ------------------------------------------------------------ |
| CPU         | AMD Ryzen 5 5500H                                           |
| Memory      | 16 GB SO-DIMM DDR4 3200MHz                                   |
| DISK        | PCIe M.2 NVMe SSD 500GB + PCIe M.2 NVMe SSD 1TB (additional) |
| Graphics    | AMD Radeon Vega Series & NVIDIA GeForce RTX 2050             |
| Monitor     | FHD 1920x1080 144Hz                                          |
| Network     | Realtek 8822CE 11AC (2x2) & Bluetooth® 5.0                   |
| Trackpad    | Synaptics                                                    |

## Compatibility Status:

| Status | Name                 | Additional Information                                                         |
| :----: | -------------------- | ------------------------------------------------------------ |
|   ❌   | WiFi                | While the Wifi doesn't work, you can use Android USB thetering thanks to HoRNDIS.kext |
|   ✅    | Bluetooth          | Works flawlessly thanks to BlueToolFixup.kext |
|   ✅    | USB's                 | All USB's work just fine, they've been mapped with USBMap   |
|   ✅    | Keyboard + Backlight  | Works without no issues at all |
|   ✅    | Speakers                 | Speakers are working without an issues   |
|   ✅    | Microphone                 |   |
|   ✅    | Webcam                |                                    |
|   ❌    | Trackpad + Gestures      | Trackpad unfortunately doesn't work   |
|   ✅    | Battery + Status               |                                    |
|   ✅    | HDMI               |    |
|   ❌    | NVIDIA GeForce RTX 2050               |  No driver  |
|   ✅    | AMD Radeon Vega Series               |  Fully working with macOS with NootedRed.kext, full 3D acceleration!  |
