# NUC8I5BEH 黑苹果 (OpenCore)

[English](./README.md) | 简体中文

### 支持的macOS版本
+ macOS Mojave
+ macOS Catalina
+ macOS Big Sur
+ macOS Monterey
+ macOS Ventura
+ macOS Sonoma
+ macOS Sequoia

OpenCore: `1.0.1`

如果你已升级到 Sonoma（或更高）且有使用 Wi-Fi 的需求，请参考以下资料
+ [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher/) (白果网卡)
+ [OpenIntelWireless](https://github.com/OpenIntelWireless/itlwm/) (自带的英特尔网卡)

### BIOS设置
+ __禁用__
	- Legacy Boot
	- Fast Boot
	- Network Boot
	- Secure Boot
	- Inter VT for directed I/VO(VT-d)
+ __启用__
	- Boot USB Devices First
	- Boot Network Devices Last
+ __Wake on LAN from S4/S5__
	- Stay Off


### 使用方法
1. 将 **EFI** 和 **NUC8_MacOnlineInstaller** 放入FAT32 U盘根目录
2. 根据操作系统，执行**NUC8_MacOnlineInstaller**中对应的run脚本
3. 以上步骤完成后关机，使用U盘安装系统

### 激活iMessage/FaceTime
1. 使用[Hackintool](https://github.com/headkaze/Hackintool)生成**Serial Number**, **Board Serial Number** 和 **SmUUID**
2. 在[https://checkcoverage.apple.com](https://checkcoverage.apple.com)查询你的**Serial Number**，并确保查询结果如下图所示，否则继续摇号
![checkSN](checkSN.png)
3. 在 *config.plist* 中替换它们
4. 重启电脑

---

## Show your support

Give a ⭐️ if this project helped you!
