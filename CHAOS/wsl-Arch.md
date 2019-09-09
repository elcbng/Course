# Windows Subsystem for ArchLinux
> 来自 yuk7 的 [**这个repo**](https://github.com/yuk7/ArchWSL)

## 启用wsl
!你必须使用 Windows 10.0.16215.1000 或者以后的版本

使用管理员权限运行 powershell
输入以下命令
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

重启Windows

## 从 yuk7 的 [**Releases**](https://github.com/yuk7/ArchWSL/releases) 下载打包好的Arch

> https://github.com/yuk7/ArchWSL/releases/download/19.7.2.0/ArchWSL-AppX_19.7.2.0_x64.appx
> https://github.com/yuk7/ArchWSL/releases/download/19.7.2.0/ArchWSL-AppX_19.7.2.0_x64.cer

## 安装
1. 使用管理员权限安装 .cer 证书到**本地计算机**的**受信任的根证书颁发机构**
1. 双击 .appx 安装 ArchWSL

## 后续步骤
### 更新 archlinux-keyring
Please follow ArchWiki 的 [这篇文章](https://wiki.archlinux.org/index.php/Pacman/Package_signing)