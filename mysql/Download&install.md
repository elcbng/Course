# 环境搭建/下载wamp与安装
## 下载WAMP
### 官网下载
1. [wampserver官方网站](http://www.wampserver.com/en/#download-wrapper)  
![Alt text](img\wampdownload.png)  
~~这里应该有一张图片~~  
1. 根据自己版本下载对应的版本64位系统下载64位版本  
32位系统下载32位版本  
### 百度网盘下载  
1. [百度云](www.baidu.com)  
提取码：
~~这里我还没上传~~
## 安装wampserver  
1. 打开下载好的wamp安装包
![Alt text](img\wampinstall.png)  
~~这里应该有一张图片~~
1. 一路点next
![Alt text](img\wampnext.png)  
1. 完成安装
## 启动wampserver
1. 点击启动wampserver  
![Alt text](img\wampclick.png)  
期间会弹出一些命令行弹窗  
1. 若wamp所以服务正常运行将在状态栏看到一个绿色图标  
![Alt text](img\wamprun.png)   
鼠标停留在上会显示所有服务正常运行  
若为红色则没有一个服务正常运行  
为橙色则为部分服务未正常运行  
未正常运行时慢慢排查问题所在  
1. 打开浏览器输入[localhost](localhost)  
将看到以下界面则说明apache服务器运行成功  
并可在界面中查看MySQL版本  
![Alt text](img\wamplocalhost.png)   
## 修改MySQL服务密码   
1. 点击Your Aliases下的phpmyadmin  
![Alt text](img\clickadmin.png)   
1. 进入[phpMyAdmin](http://localhost/phpmyadmin/)  
1. 默认密码为空点击执行
![Alt text](img\phpmyadminpage.png)   
1. 进入界面后点击顶端导览的账户后点击修改权限  
![Alt text](img\roothomepage.png)   
1. 点击修改密码  
输入自己能记住的密码  
最好是4位纯数字密码  
太长以后打开你会嫌烦的  
![Alt text](img\clickchange.png)   
- 以上修改密码步骤后可用终端完成
- 若一开始上终端无休止打错东西
- 可能会劝退很多人
