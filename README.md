# NUC8I5BEH Hackintosh (OpenCore)

English | [简体中文](./README-zh_CN.md)

### Supported macOS versions
+ macOS Mojave
+ macOS Catalina
+ macOS Big Sur
+ macOS Monterey
+ macOS Ventura
+ macOS Sonoma
+ macOS Sequoia

OpenCore: `1.0.1`

If you've upgraded to Sonoma (or later) and have a need for Wi-Fi, please refer to the following
+ [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher/) (for Mac official NIC)
+ [OpenIntelWireless](https://github.com/OpenIntelWireless/itlwm/) (for the Intel NIC that came with it)

### BIOS Settings
+ __Disable__
	- Legacy Boot
	- Fast Boot
	- Network Boot
	- Secure Boot
	- Inter VT for directed I/VO(VT-d)
+ __Enable__
	- Boot USB Devices First
	- Boot Network Devices Last
+ __Wake on LAN from S4/S5__
	- Stay Off


### How to install
1. Put **EFI** and **NUC8_MacOnlineInstaller** into a Fat 32 format USB flash driver's **root directory**
2. Run the corresponding script file in **NUC8_MacOnlineInstaller** depending on your operating system
3. Restart computer and install macOS with the USB flash driver After all steps above are completed

### Active iMessage/FaceTime
1. Genarate **Serial Number**, **Board Serial Number** and **SmUUID** with [Hackintool](https://github.com/headkaze/Hackintool)
2. Check your **Serial Number** on [https://checkcoverage.apple.com](https://checkcoverage.apple.com), and make sure the result looks like the picture below, otherwise genarate them again (and again)
![checkSN](checkSN.png)
3. Replace **Serial Number**, **Board Serial Number** and **SmUUID** in *config.plist*
4. Restart computer

---

## Show your support

Give a ⭐️ if this project helped you!
