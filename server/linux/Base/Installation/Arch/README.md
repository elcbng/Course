# ArchLinux 的安装教程

你去看 [**ArchWiki**](https://wiki.archlinux.org/index.php/Installation_guide_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)) 啊！

## 额外步骤
其实ArchWiki有一些东西没有强调出来，为了防止在安装之后翻车，所以有一些额外的步骤最好还是跟你们说一下比较好。

在pacstrap之前，先更换为中国境内的的源，来加速安装时下载软件的过程。

软件源的配置通过修改 **/etc/pacman.d/mirrorlist** 文件即可。

``` bash
nano /etc/pacman.d/mirrolist
```

