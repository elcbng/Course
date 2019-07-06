# Linux

<details>
<summary><b>简介</b></summary>
<p><a href="Base">跳转到“<b>简介</b>”分节</a></p>
<pre><code>
  - 声明
  - Linux 发行版
  - Init相关
</code></pre>
</details>

## 基础
<details>
<summary><b>安装</b></summary>
<pre><code>
  - Ubuntu 乌班图
  - CentOS
  - ArchLinux
  - <s>Openwrt</s>
  - <s>Gentoo(等待勇士填坑)</s>
</code></pre>
</details>

<details>
<summary><b>初步使用 Linux</b></summary>
<pre><code>
  - Desktop Manager 桌面管理器
  - Desktop Environment 桌面环境
  - 软件包管理系统
    - Debian dpkg
      - apt 前端
    - Fedora rpm
      - <s>dnf 前端</s>
      - yum 前端
    - Arch pacman
      - Arch AUR
        - yay 前端
    - <s>Gentoo portage</s>
    - Openwrt opkg
    - <s>额外</s>
      - <s>macOS homebrew</s>
      - <s>Chromium chromebrew</s>
      - <s>Windows Installer</s>
        - <s>Windows Installer 前端</s>
        - <s>Chocolatey 前端</s>
  - daemon
    - <s>System V</s>
    - systemd 底裤
      - "d"
  - iptables
    - UFW 前端
</code></pre>
</details>

## 高级

<details>
<summary><b>Linux 的启动</b></summary>
<pre><code>
  - Bootloader
    - UEFI
      - Grub
      - Syslinux
      - Systemd Boot 底裤启动
      - <s>EFISTUB</s>
        - <s>rEFInd</s>
        - <s>Clover 四叶草</s>
    - <s>Legacy</s>
      - <s>Grub Legacy</s>
      - <s>Grub</s>
      - <s>Syslinux</s>
      - <s>Grub4dos</s>
    - <s>额外补充内容：嵌入式</s>
      - <s>U-Boot</s>
      - <s>Breed（路由器）</s>
  - rootfs
    - initramfs
  - Init
</code></pre>
</details>

<details>
<summary><b>Linux 的结构</b></summary>
<pre><code>
  - 文件系统
    - 分区格式
    - “/”的下面是宇宙
  - "/"
    - /boot 启动
    - /dev 设备
    - /sys 系统
    - /bin & /sbin 二进制可执行文件
    - /lib % /lib64 库
    - /opt
    - /root 跟用户目录
    - /home 用户目录
    - /usr
    - /etc
    - /mnt
    - /proc
    - /run
    - /srv
    - /var
    - /tmp
  - “逻辑上”的结构
    - Hardware 硬件
    - Kernel 内核
      - Kernel Space 内核空间
        - Kernel Modules 内核模块
        - 子系统
        - 内核接口
      - User Space 用户空间
        - C标准库
        - daemon 系统守护进程
        - 窗口系统
        - 图形驱动程序
        - Lib 其他库
        - App 应用程序
    - CoreUtils 核心工具链
    - Shell
</code></pre>
</details>

<details>
<summary><b>Linux 能有多骚</b></summary>
<p><a href="Advanced">跳转到“<b>Linux 能有多骚</b>”目录</a></p>
<pre><code>
  很简单，要多骚有多骚
</code></pre>
</details>
