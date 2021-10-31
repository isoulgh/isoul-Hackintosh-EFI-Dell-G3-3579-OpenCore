# isoul-Hackintosh-EFI-Dell-G3-3579-OpenCore

# OC版本0.7.4--macOS12.0.1
这是我使用的EFI备份，也欢迎各位hxd借鉴，提出宝贵的意见，嘻嘻。

## Features
1. 可用Thunderbolt口任意外接显示器
2. Thunderbolt口的其他功能需添加额外一个Kext并且有Bug不建议使用
3. HDMI口直连独显，独显在Mac下无法驱动，故无法使用
4. 博通网卡直接使用，其他网卡只需替换一下网卡驱动即可
5. 使用dw1560网卡，Mac所有特色功能全支持（包括watch解锁，智能热点，随航，接力，隔空投送等所有功能，可登陆AppleID）
6. 我的详细配置如下：

## 我的电脑配置

|   配件   |             规格              | 工作状态 |
| :------: | :---------------------------: | :------: |
|   模组   |         Dell G3 3579          |    ✅     |
|  处理器  | Intel Core i7-8750H |    ✅     |
|   内存   |    威刚8GB*2 DDR4 2666Mhz    |    ✅     |
| 固态硬盘 |   Samsung 970Pro 512GB   |    ✅     |
| 机械硬盘 |         原装希捷 1TB        |    ✅     |
| 核芯显卡 |    Intel UHD Graphics 630    |    ✅     |
| 独立显卡 |  NVIDIA GeForce GTX 1060 MaxQ  |    🚫     |
|   声卡   |        Realtek ALC236         |    ✅     |
| 有线网卡 |        Realtek RTL8111        |    ✅     |
| 无线网卡 |     Broadcom 94352Z（DW1560）     |  ✅  |

## BIOS 设置

| **System Configuration** |      |
| --- | --- |
| SATA Operation       | AHCI |
|                      |      |
| **Secure Bootxu**   |      |
| Secure Boot Enable   | Disabled（取消勾选） |
|  |                    |
| **Intel Software Guard Extensions** |                    |
| Intel SGX Enable | Disabled           |
|  |                    |
| **POST Behavior** |                    |
| Fastboot | Thorough           |
|  |                    |
| **Virtualization Support** |                    |
| VT for Direct I/O | Disabled（取消勾选） |

请更新 BIOS 至最新版本！

其他保持默认设置。

## 工作的部分

- macOS 12.x（经测试可直升）
- CPU
- 核心显卡
- 有线网卡
- 音频（Layout=15）
- USB（定制USBPorts.kext）
- 触摸板
- 摄像头
- 蓝牙
- Wi-Fi
- Thunderbolt（使用需自行添加IOExxx.kext，名字忘了，有bug）
- Thunderbolt外接显示器可热拔插任意使用

## 不工作的部分

- 独立显卡（已禁用）
- HDMI
- 内置读卡器（未测试，应该能用）
