### HP ProBook 6470b EFI Ventura Official Nightly Builds

**EFI for MacOS Ventura on HP ProBook 6470b (2012)**🎉

I am thrilled to share my successful Hackintosh project on my 2012 HP ProBook 6470b! Running MacOS Ventura without a hitch, this old machine has been revitalized and is performing exceptionally well. Below are the specs and details of the setup:


### 🖥️ System Specifications:


- 💻 CPU Type: Mobile DualCore Intel Core i5-3320M, 3100 MHz (31 x 100)
- 🔧 Motherboard Chipset: Intel Panther Point HM76, Intel Ivy Bridge
- 🎨 Video Adapter: Intel(R) HD Graphics 4000 (2112 MB)
- 🔊 Audio Adapter:
- IDT 92HD81B1X @ Intel Panther Point PCH - High Definition Audio Controller [C1]
- Intel Panther Point HDMI @ Intel Panther Point PCH - High Definition Audio Controller [C1]
- 🌐 Network Adapter:
- Intel(R) 82579V Gigabit Network Connection
- Intel(R) Centrino(R) Advanced-N 6205
- 🔥 FireWire Controller: JMicron JMB380 PCI-E 1394a OHCI FireWire Controller and Memory Card Host Controller
- 🔌 USB Device:
- Broadcom 20702 Bluetooth 4.0 Adapter
- HP HD Webcam [Fixed]
- 💽 IDE Controller:
- Standard SATA AHCI Controller
- JMicron PCIe SD/MMC Host Controller

### ⚙️ Performance and Stability:

Despite its age, the HP ProBook 6470b runs MacOS Ventura seamlessly. Here are some highlights of the performance:

- Graphics: The Intel HD Graphics 4000 handles the macOS interface smoothly, providing a good user experience without any graphical glitches.
- Audio: Both audio adapters work perfectly, ensuring crisp and clear sound whether using the built-in speakers or external devices.
- Network: Wired and wireless connections are stable and reliable, courtesy of the Intel network adapters.
- Bluetooth & USB: The Broadcom Bluetooth adapter and various USB devices function without issues, ensuring full peripheral compatibility.
- Webcam: The integrated HP HD Webcam works flawlessly with video conferencing apps.

### 🛠️ Installation Process:

The installation was straightforward, thanks to the robust EFI configuration and available guides. Key steps included:

- 💾 Creating a Bootable USB Installer: Used a Mac or another Hackintosh to create a bootable USB with MacOS Ventura.
- 🔧 Configuring the BIOS: Ensured BIOS settings were optimized for macOS compatibility (e.g., disabling Secure Boot, enabling AHCI).
- 📁 EFI Folder Configuration: Placed the necessary kexts, drivers, and configuration files in the EFI folder.
- 💻 Installing MacOS: Booted from the USB installer, formatted the drive to APFS, and installed MacOS Ventura.
- 🛠️ Post-Installation Tweaks: Applied post-installation tweaks to ensure all hardware components were recognized and functional.
- 🗂️ EFI Configuration and Support:
- I am excited to announce that I will be providing nightly builds for the EFI folders, ensuring they are up-to-date and optimized for the best performance. Additionally, I will be offering support to assist with any issues or questions you may have.

### Here's a snapshot of the key components in my EFI folder:

### Bootloader: OpenCore (version 1.0.0)

Essential Kexts:
- Lilu.kext
- WhateverGreen.kext
- AppleALC.kext
- IntelMausi.kext
- AirportBrcmFixup.kext
- USBInjectAll.kext
- VirtualSMC.kext
- Drivers:
- OpenRuntime.efi
- HfsPlus.efi
Configuration File: A meticulously edited config.plist to match the system specifications and optimize performance.

### ✅ What's Working:

- 🛜 Wi-Fi
- 📶 Bluetooth
- 📤 Airdrop
- 🎥 HDMI
- 🎵 AUDIO
- 🌐 Ethernet
- 🔥 FireWire
- 💳 Express Cards
- 🔒 Close/Open lid
- 💡 Laptop Backlight
- 🖥️ Multiple Displays
- 📺 VGA Output port
- 🔌 USB2.0
- 🔋 USB3.0
- 🎛️ PS2 TouchPad
- 🔋 Battery? (I have no battery to test, but you can expect it should be working properly)
- 🌙 Hibernation? (Sometimes, please test and report)

### ⚠️ Known Issues:

- 📶 Bluetooth: Seems to not be compatible with iPhone devices, but other device types are compatible.
- 💬 iMessage and FaceTime: Seem to force close themselves. Make sure to add proper SN info to your config.plist and test after reinstall.
- 🖥️ Graphics: As Apple dropped support, you may get choppy graphics issues and not see properly throughout the PC screen. To avoid this during the installation process, please turn on the laptop with the screen closed and connected to a TV or monitor using the DVI port (which stands as HDMI as well in this machine). To get graphics working properly, you may need to install the OCLP app offered here to provide root patches.
- 🎛️ Trackpad: The trackpad integrated on the keyboard is not working properly, and I am still figuring out how to get it working again as it was working properly previously.
- ⚠️ More issues? You tell me...

### 🙏 Acknowledgements:

This project wouldn't have been possible without the incredible work of the Hackintosh community. Special thanks to the developers and contributors of the tools and kexts used in this project:

- OpenCore: For the powerful bootloader.
- Lilu.kext: Essential for patching macOS.
- WhateverGreen.kext: For fixing graphics issues.
- AppleALC.kext: For enabling audio support.
- IntelMausi.kext: For network compatibility.
- AirportBrcmFixup.kext: For Wi-Fi and Bluetooth functionality.
- USBInjectAll.kext: For USB support.
- VirtualSMC.kext: For hardware monitoring.
- Your dedication and hard work have made it possible to bring macOS to non-Apple hardware. Thank you!


### Images


![](https://i.imgur.com/5ck6xZA.png)

> Wi-Fi working

![](https://i.imgur.com/cFDoRvm.png)

> Springboard/Launchpad

![](https://i.imgur.com/KB7EoWq.png)

> Intel HD 4000 Driver working

![](https://i.imgur.com/TdK1Enw.png)

> About Mac

![](https://i.imgur.com/N9zbIuc.png)

> Stock Wi-Fi List


### 💖 Donations:
If you find this project helpful and would like to support its ongoing development, consider making a [donation](http://paypal.me/AlienSK "donation"). Your contributions will help cover the costs of maintaining and improving the EFI configurations, as well as providing support. Every little bit helps and is greatly appreciated.

### END
