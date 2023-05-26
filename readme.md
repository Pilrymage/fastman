# Fastman

荒野求生级安装+配置包。

## 硬件

- 二手 ThinkPad，以 x1c6 为例
- 2TB SSD 作系统盘，国产 SSD 在价格上肉眼可见的内卷
- HDMI-DVI 线，可以接显示器，适用于学校里有方便插拔显示器的台式机
- 1TB microSD，空间大，体积小到可以放入钱包数张
- 4TB 移动硬盘，考虑做备份

## 操作系统

- Windows 10 LTSC IoT，可以支持到 2032 年（本仓库的未来九年）。
- Gentoo Linux，超高的自定义能力。
- 使用 OpenCore 的 Hackintosh （黑苹果，Monterey），对 x1c6 ThinkPad 的支持很好。
- FreeBSD，体验 Linux 之外的风情。

### 分区

- sda1：boot启动分区，200M，
- sda2：EFI 分区，300M，使用 MiniTool Partition Wizard 在安装后扩容
- sda3：Windows 恢复分区，16M（默认）
- sda4：Windows 系统盘，150G+10M
- sda5: 交换分区，10G
- sda6: Gentoo Linux 系统盘，80G
- sda7: MacOS 系统盘，150G
- sda8: FreeBSD 系统盘，60G
- sda9: 数据盘
- （留个200G）

### 安装

- 安装 Windows。参见[友好Windows讨论串](https://rentry.org/fwt)。
  [磁力](magnet:?xt=urn:btih:29e10fd1688e053aa6a311c31847503ba730772e&dn=Microsoft+Windows+10+IoT+Enterprise+LTSC+2021,+Version+21H2+-+%D0%9E%D1%80%D0%B8%D0%B3%D0%B8%D0%BD%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5+%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D1%8B+%D0%BE%D1%82+Microsoft+MSDN+%5BEn%5D&tr=udp://tracker.openbittorrent.com:80&tr=udp://tracker.opentrackr.org:1337/announce)或[种子](https://isofiles.bd581e55.workers.dev/Windows%2010/Windows%2010%20Enterprise%20LTSC%202021/)下载 Windows 镜像，以及[rufus](https://rufus.ie/en/).
- 安装 Gentoo Linux. 参见[Gentoo Linux 安装及使用指南](https://bitbili.net/gentoo-linux-installation-and-usage-tutorial.html)
.
- 安装 MacOS。参见[OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)以及[x1c6-hackintosh](https://tylernguyen.github.io/x1c6-hackintosh/).
- 安装 [FreeBSD](https://www.freebsd.org/).

## Windows 装机

安装操作系统：安装界面很容易。
多出10MB专为强迫症患者服务。
将Windows的用户文件夹移到移到
安装软件：scoop安装。

## MacOS 装机

安装操作系统：使用EFI。