# Fastman

荒野求生级安装+配置包。

## 硬件

- 二手 ThinkPad，以 x1c6 为例
- 2TB SSD 作系统盘，国产 SSD 在价格上肉眼可见的内卷
- HDMI-DVI 线，可以接显示器
- 1TB microSD，空间大，体积小到可以放入钱包数张

## 操作系统

- Windows 10 LTSC IoT，可以支持到 2032 年（本仓库的未来九年）。
- Gentoo Linux，超高的自定义能力。
- 使用 OpenCore 的 Hackintosh （黑苹果），对 x1c6 ThinkPad 的支持很好。
- FreeBSD，体验 Linux 之外的风情。

### 分区

- sda1: EFI partition, 300M
- sda      8:0    0 476.9G  0 disk 
├─sda1   8:1    0   300M  0 part /boot/efi
├─sda2   8:2    0    16M  0 part 
├─sda3   8:3    0   145G  0 part 
├─sda4   8:4    0   105G  0 part 
├─sda5   8:5    0   500M  0 part /boot
├─sda6   8:6    0     8G  0 part 
├─sda7   8:7    0   150G  0 part /
├─sda8   8:8    0   200M  0 part 
└─sda9   8:9    0    30G  0 part 
