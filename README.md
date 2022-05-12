# isoul-Hackintosh-EFI-Dell-G3-3579-OpenCore

# OC 0.7.8--macOS 12.2.1
这是我使用的EFI备份，欢迎各位hxd借鉴，提出宝贵的意见，嘻嘻。

## Notes
1. 无线网卡驱动请自行添加。
2. BIOS设置见下文。
3. 三星部分硬盘启动或安装速度较慢，请耐心等待。（时间长短不一，因Trim机制与苹果系统有冲突）

## Features
1. 可用Thunderbolt口任意外接显示器
2. Thunderbolt口的其他功能需添加额外一个Kext并且有Bug不建议使用
3. Mac所有特色功能全支持（包括watch解锁，智能热点，随航，接力，隔空投送等所有功能）
4. macOS 12.x（经测试可直升）
5. 音频（Layout=15）
6. USB（定制USBPorts.kext）


### 我的电脑配置

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
| 无线网卡 |     Broadcom 94360NG(免驱)     |  ✅  |

### BIOS 设置

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

其他保持默认设置即可。


### 不工作的部分

- 独立显卡（已禁用）
- HDMI（连在独显上）
- 读卡接口（未测试，应该能用）
