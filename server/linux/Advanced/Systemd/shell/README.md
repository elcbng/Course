# Systemd 命令

## Systemd 基本工具

### 检查
显示系统状态
``` shell
systemctl status
```

输出激活的单元
``` shell
systemctl
```

输出运行失败的单元
``` shell
systemctl --failed
```

查看所有已安装服务
``` shell
systemctl list-unit-files
```

### 管理

立即激活单元
``` shell
systemctl start <unit>
```

立即停止单元
``` shell
systemctl stop <unit>
```

立即重启单元
``` shell
systemctl restart <unit>
```

输出单元状态
``` shell
systemctl status <unit>
```

开机启动单元
``` shell
systemctl enable <unit>
```

设置开机启动单元，并现场启动
``` shell
systemctl enable --now <unit>
```

取消开机启动单元
``` shell
systemctl disable <unit>
```
>其余详见[Archwiki](https://wiki.archlinux.org/index.php/Systemd_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)#systemd_%E5%9F%BA%E6%9C%AC%E5%B7%A5%E5%85%B7)


# Systemd logging system: journal
#### 读取日志
``` shell
journalctl
```

#### 过滤输出
详见 [Archwiki](https://wiki.archlinux.org/index.php/Systemd/Journal_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)#%E8%BF%87%E6%BB%A4%E8%BE%93%E5%87%BA)