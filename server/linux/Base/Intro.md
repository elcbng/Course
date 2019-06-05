# Linux
[维基](https://zh.wikipedia.org/wiki/Linux)
[Wiki](https://en.wikipedia.org/wiki/Linux)

本篇章将介绍各种基于Linux内核的操作系统，并深入介绍GNU/Linux

### 声明：

* 本人只会按照自己认为用得到的方面进行讲解

* 在讲解过程中将会使用[**Ubuntu**](https://en.wikipedia.org/wiki/Ubuntu)([**乌班图**](https://zh.wikipedia.org/wiki/Ubuntu))，[**CentOS**](https://en.wikipedia.org/wiki/CentOS)[(中文)](https://zh.wikipedia.org/wiki/CentOS)，[**Archlinux**](https://wiki.archlinux.org/index.php/)三个**Linux发行版**作为例子。

* 本篇默认你使用[GRUB](https://en.wikipedia.org/wiki/GNU_GRUB)[引导加载器](https://zh.wikipedia.org/wiki/GNU_GRUB)来引导并加载Linux发行版。
  - 注：关于使用[rEFInd](https://wiki.archlinux.org/index.php/REFInd) [(中文)](https://wiki.archlinux.org/index.php/REFInd_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87))或者[Clover](https://wiki.archlinux.org/index.php/Clover) [(中文)](https://wiki.archlinux.org/index.php/Clover_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87))，[Systemd Boot](https://wiki.archlinux.org/index.php/Systemd-boot) [(中文)](https://wiki.archlinux.org/index.php/Systemd-boot_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87))的教程也可能会涉及。

* 本篇可能会涉及路由器的[**OpenWRT**](https://openwrt.org/) [(Wiki)](https://zh.wikipedia.org/wiki/OpenWrt)

## [Distribution](https://en.wikipedia.org/wiki/Linux_distribution) [发行版](https://zh.wikipedia.org/wiki/Linux%E5%8F%91%E8%A1%8C%E7%89%88)

**Linux 发行版**（英语：**Linux distribution**），为一般用户预先集成好的Linux操作系统及各种应用软件。一般用户不需要重新编译，在直接安装之后，只需要小幅度更改设置就可以使用，通常以软件包管理系统来进行应用软件的管理。Linux发行版通常包含了包括桌面环境、办公包、媒体播放器、数据库等应用软件。这些操作系统通常由Linux内核、以及来自GNU计划的大量的函数库，和基于X Window的图形界面。有些发行版考虑到容量大小而没有预装 X Window，而使用更加轻量级的软件，如：busybox, uclibc 或 dietlibc。现在有超过300个Linux发行版(Linux发行版列表)。大部分都正处于活跃的开发中，不断地改进。

### **Linux发行版**可以认为有以下的分支：

#### 手上的Linux(非GNU/Linux)
- Android 安卓
  - GMS Android (注：这是一部分人定义的“拥有完整谷歌服务的Android”)
    - Android IA
    - Android TV
    - Wear OS
  - Android Open Source Project(AOSP) 安卓开源计划 (默认不包含谷歌服务，可自行安装)
    - Android x86
    - Cyaongen Mod
      - Cyaongen OS
      - Lineage OS
    - Mokee 魔趣开源项目
    - OmniROM
    - Resurrection Remix OS
  - Android ONE

#### 计算机上的Linux(GNU/Linux)
- Arch
  - Manjaro (非官方中文名：麻将)
- Debian
  - Ubuntu 乌班图
    - Ubuntu Touch
    - Ubuntu Server
    - UbuntuKylin 优麒麟
      - NeoKylin 中标麒麟
    - Linux Mint
    - KDE Neon
      - Plasma Mobile
  - Deepin 深度
  - Kali Linux
    - Kali Linux NetHunter
- Red Hat 红帽
  - Fedora Core
    - Fedora
      - Red Star OS 붉은별 红星
      - Moblin 2
        - MeeGo
          - Mer
            - Sailfish OS 旗鱼
          - Tizen
  - Red Hat Enterprise
    - CentOS
- Enoch
  - Gentoo
    - Chrome OS
      - Chromium OS
- Slackware
  - S.u.S.E
    - SuSE
      - SUSE
        - openSUSE
- 鸿蒙 Hongmeng OS、HomonOS、HMOS
- 红旗Linux

#### 路由器上的Linux(GNU/Linux)
- OpenWRT
  - LEDE
  - Asuswrt
    - Merlin 梅林
- DD-WRT
- Tomato

因为[Linux发行版分支图](https://github.com/CerteKim/BNG/blob/master/server/linux/img/Linux_distribution.png)面积太大，所以不在这里贴出，但给出链接供参考。  

## [Init](https://en.wikipedia.org/wiki/Init) [(中文页面)](https://zh.wikipedia.org/wiki/Init)
由于本人能力有限，并不会讲解 [__UNIX System III__](https://zh.wikipedia.org/wiki/UNIX_System_III) 、 [__UNIX System V__](https://zh.wikipedia.org/wiki/UNIX_System_V) 或者 [__Upstart__](https://zh.wikipedia.org/wiki/Upstart)

所以只讲解[**Systemd**](https://zh.wikipedia.org/wiki/Systemd)