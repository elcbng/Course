# Linux
[**维基**](https://zh.wikipedia.org/wiki/Linux)
[**(Wiki)**](https://en.wikipedia.org/wiki/Linux)

>本篇章将介绍各种基于 **Linux 内核** 的操作系统，并深入介绍 GNU/Linux

>**Linux** 是一种自由和开放源码的 **类 UNIX** 操作系统。该操作系统的内核由**林纳斯·托瓦兹**在1991年10月5日首次发布，在加上用户空间的应用程序之后，成为 Linux 操作系统。Linux 也是自由软件和开放源代码软件发展中最著名的例子。

*只要遵循 **GNU 通用公共许可证（GPL）** ，任何个人和机构都可以自由地使用 Linux 的所有底层源代码，也可以自由地修改和再发布。* 

>大多数 Linux 系统还包括像提供 GUI 的 X Window 之类的程序。

__*除了一部分专家之外，大多数人都是直接使用 Linux 发行版，而不是自己选择每一样组件或自行设置。*__

<br><br>
1991 年 10 月 5 日， **Linus Torvalds** 首次发布 **Linux 内核** 。 Linux 内核是 Linux 系统的一个非常重要的组成部分。目前， Linux 主要用于多种服务器和超级计算机等。它也被用于手机操作系统，比如 Android 操作系统是基于 Linux 内核的。

<br><br>
在早期，Linux 作为一个免费的操作系统被用于基于 Intel ×86 的个人电脑上。因为 Linux 是一个开源操作系统，所以它的源代码可以被修改或使用，也可以在有 **GPL（通用公共许可证）** 这样许可证下被任何人发布。简而言之，如果具备一定知识，知道自己在干什么，那么任何人都可以从 Linux 那儿获得自己的操作系统。正因此，才有了许多 Linux 发行版。

<br>

### [Distribution](https://en.wikipedia.org/wiki/Linux_distribution) [发行版](https://zh.wikipedia.org/wiki/Linux%E5%8F%91%E8%A1%8C%E7%89%88)

**Linux 发行版**（英语：**Linux distribution**），为一般用户预先集成好的 Linux 操作系统及各种应用软件。一般用户不需要重新编译，在直接安装之后，只需要小幅度更改设置就可以使用，通常以软件包管理系统来进行应用软件的管理。Linux 发行版通常包含了包括桌面环境、办公包、媒体播放器、数据库等应用软件。这些操作系统通常由 Linux 内核、以及来自 GNU 计划的大量的函数库，和基于 X Window 的图形界面。有些发行版考虑到容量大小而没有预装 X Window，而使用更加轻量级的软件，如：busybox, uclibc 或 dietlibc 。现在有超过300个 Linux 发行版( Linux 发行版列表)。大部分都正处于活跃的开发中，不断地改进。


### **Linux 发行版** 可以认为有以下的分支：

<details>
<summary><b>手上的 Linux(非GNU/Linux)</b></summary>
<pre><code>
  - Android 安卓
  - GMS Android (注：这是一部分人定义的“拥有完整谷歌服务的 Android ”)
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
</code></pre>
</details>

<details>
<summary><b>计算机上的 Linux(GNU/Linux)</b></summary>
<pre><code>
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
</code></pre>
</details>

<details>
<summary><b>路由器上的 Linux</b></summary>
<pre><code>
- OpenWRT
  - LEDE
  - Asuswrt
    - Merlin 梅林
- DD-WRT
- Tomato
</code></pre>
</details>

<br>

因为 [Linux 发行版分支图](img/Linux_distribution.png)面积太大，所以不在这里贴出，但给出链接供参考。  


--------------
### 声明：

* 本人只会按照自己认为用得到的方面进行讲解

* 在讲解过程中将会使用 [**Ubuntu**](https://en.wikipedia.org/wiki/Ubuntu)([**乌班图**](https://zh.wikipedia.org/wiki/Ubuntu))，[**CentOS**](https://en.wikipedia.org/wiki/CentOS)[(中文)](https://zh.wikipedia.org/wiki/CentOS)，[**Archlinux**](https://wiki.archlinux.org/index.php/) 三个 **Linux 发行版**作为例子。

* 本篇默认你使用 [GRUB](https://en.wikipedia.org/wiki/GNU_GRUB)[引导加载器](https://zh.wikipedia.org/wiki/GNU_GRUB) 来引导并加载 Linux 发行版。
  - 注：关于使用 [rEFInd](https://wiki.archlinux.org/index.php/REFInd) [(中文)](https://wiki.archlinux.org/index.php/REFInd_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)) 或者 [Clover](https://wiki.archlinux.org/index.php/Clover) [(中文)](https://wiki.archlinux.org/index.php/Clover_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87))，[Systemd Boot](https://wiki.archlinux.org/index.php/Systemd-boot)  [(中文)](https://wiki.archlinux.org/index.php/Systemd-boot_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)) 的教程也可能会涉及。

* 本篇可能会涉及路由器的 [**OpenWRT**](https://openwrt.org/) [(Wiki)](https://zh.wikipedia.org/wiki/OpenWrt)

* 由于本人能力有限，并不会讲解 [__UNIX System III__](https://zh.wikipedia.org/wiki/UNIX_System_III) 、 [__UNIX System V__](https://zh.wikipedia.org/wiki/UNIX_System_V) 或者 [__Upstart__](https://zh.wikipedia.org/wiki/Upstart)
<br>所以只讲解 [**Systemd**](https://zh.wikipedia.org/wiki/Systemd)

# 继续阅读，请前往：[目录](base.md)