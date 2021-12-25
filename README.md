# X270 Hackintosh - OpenCore - i7-7500U - Big Sur
This repo contains the files and scripts to install macOS on the Lenovo X270 family

A fork of [michaeldigiacomi´s X270](https://github.com/michaeldigiacomi/Lenovo-X270-Hackintosh-OpenCore)

With special thanks to [taida2203´s fork for i7-7500U](https://github.com/taida2203/Lenovo-X270-Hackintosh-OpenCore)

This seeks to change and add a few things, notably, the touchpad and the physical buttons, which now include working [gestures](Images/gestures.gif). taida2203´s fork contains Realtek drivers, whereas this one is for Intel (with HeliPort)

If you´re running a X270 with any other CPU and you´re simply looking for gestures fix - replace VoodooPS2Controller.kext from this repo with your own.


There is a slight hiccup with the Bluetooth looping a bit much, but with patience it goes through, alternatively just disable it.



![X270](Images/a-screen.png)

# Tested OS
- [x] macOS 11.6.2

# Laptop's Hardware
- <b>Model</b>: Thinkpad X270
- <b>Bios</b>: 1.43
- <b>CPU</b>: Intel(R) Core(TM) i7-7500U
- <b>GPU</b>: Intel HD Graphics 620
- <b>RAM</b>: 16 GB 2133MHz DDR4
- <b>Screen</b>: 14" FHD (1920x1080) IPS
- <b>Wi-Fi</b>: Intel AC 8260
- <b>Camera</b>: 720p
- <b>Battery</b>: 6-cell

# Bios settings

<b>Security</b>
- `Security Chip` **Disabled**
- `Memory Protection -> Execution Prevention` **Enabled**
- `Virtualization -> Intel Virtualization Technology` **Enabled**
- `Virtualization -> Intel VT-d Feature` **Enabled**
- `Anti-Theft -> Computrace -> Current Setting` **Disabled**
- `Secure Boot -> Secure Boot` **Disabled**
- `Intel SGX -> Intel SGX Control` **Disabled**
- `Device Guard` **Disabled**

<b>Startup</b>
- `UEFI/Legacy Boot` **UEFI Only**
- `CSM Support` **No**

# What's Working?
- [x] Intel Ethernet port
- [x] Wi-Fi & Bluetooth (including Apple services)
- [x] Intel HD 620 Graphics (incuding graphics acceleration)
- [x] CPU Power Management
- [x] Battery
- [x] All USB ports
- [x] Internal camera (including Facetime)
- [x] Realtek Audio (including headphones jack)
- [x] HDMI port (including HDMI Audio)
- [x] Keyboard (incuding all fn Keys)
- [x] Trackpad & Physical Buttons (including gestures)
- [x] Shutdown / Reboot 
- [x] iMessage, FaceTime, App Store, iTunes Store (with valid smbios)
- [x] DRM support (iTunes Movies, Apple TV+, Amazon Prime and Netflix*, and others)       *Not in Safari
- [x] SD Card Reader (v2.2 works but still a bit unstable)

# Not tested
- Dock
- AirDrop
- Sidecar

# What's not working ⚠️
- [x] Sleep / Wake (lid sleep and lid wake)

# Future
- [x] [Update OpenCore](https://github.com/aerowa/X270-Monterey-OpenCore)
- [ ] Add lid sleep/wake
- [ ] Change from itlwm to airportitlwm

# Other
- [corpnewt - MountEFI & GenSMBIOS](https://github.com/corpnewt)
- [HeliPort](https://github.com/OpenIntelWireless/HeliPort)
- [OpenCore](https://dortania.github.io/OpenCore-Install-Guide/)



