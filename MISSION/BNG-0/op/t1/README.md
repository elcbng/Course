# 第一题

## 前请概要

### Shell
Shell 是命令行，也可以编程。

例如：
```
echo 准备好开始循环了吗!
echo "#!/bin/bash" >> run.sh
chmod +x run.sh
echo "echo 循环中" >> run.sh
echo "bash run.sh" >> run.sh
bash run.sh
```

### Shell echo
以下是一个输出：```Hello World!```的 Shell 程序代码：
```shell
echo "Hello World!"
```

输出：
```shell
Hello World!
```

### 输入/输出重定向
| 命令 | 说明 |
| ---- | ---- |
| ```命令``` ```>``` ```文件``` | 输出重定向并覆盖到文件 |
| ```命令``` ```<``` ```文件``` | 输入重定向到文件 |
| ```命令``` ```>>``` ```文件``` | 输出重定向并追加到文件尾 |

### 基本文件操作
#### 复制
复制 file1 到 file2
```bash
cp file1 file2
```

#### 删除
```bash
rm file
```

#### 移动
```bash
mv file1 file2
```

#### 查看文件夹下所有文件
```bash
ls
```
例：输出：
```
桌面
文档
视频
照片
用户
网络组招新笔试题目.docx
```

## 题目
请编写一个 Shell 脚本，  
将 `我的文件夹下面有：` 和 **当前目录下所有文件名字** 输出到指定的文件，文件名随意

**例如：**
我的目录.txt：
```
我的文件夹下面有：
bin
home
dev
etc
system
```