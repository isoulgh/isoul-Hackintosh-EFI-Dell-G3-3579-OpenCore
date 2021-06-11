# OC版本0.7.0

## 电脑配置

|   配件   |             规格              | 工作状态 |
| :------: | :---------------------------: | :------: |
|   模组   |         Dell G3 3579          |    ✅     |
|  处理器  | Intel Core i7-8750H |    ✅     |
|   内存   |    16GB DDR4 2666Mhz    |    ✅     |
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

- macOS 11.4
- CPU
- 核心显卡
- 有线网卡
- 音频（Layout=15）
- USB（定制USBPorts.kext）
- 触摸板
- 摄像头
- 蓝牙
- Wi-Fi
- Thunderbolt（接着设备开机后可热拔插暂时使用，接着设备睡眠后可用，睡眠后雷电失效）
- Thunderbolt外接显示器可用（MacBookPro15,2）
- 注意：未添加机型信息，请自行添加，可添加为MacBookPro15,2

## 不工作的部分

- 独立显卡
- HDMI
- 内置读卡器（未测试）