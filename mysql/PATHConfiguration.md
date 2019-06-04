# 环境搭建/PATH环境变量配置
- 作者Cerbur

- 由于wamp服务是全服务器服务  
想单独使用MySQL还得每次运行wamp  
过于繁琐  
- 为了一劳永逸  
将MySQL加入到环境中  
此后便无需运行wamp即可使用MySQL
## 打开 Windows 环境变量配置设置
1. 使用快捷键 Win + Q 调出搜索  
1. 输入编辑系统环境变量    
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/searchpath.png)  
1. 点击环境变量  
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/pathhomepage.png)   
1. 在环境变量界面中  
下方的系统变量中  
找到 Path  
点击选中后点击编辑  
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/pathpage.png)   
## 找到MySQL所在的路径  
1. 找到安装 wamp 时候 apache 界面读取到的  
MySQL版本这里是5.7.24  
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/wamplocalhost.png)    
1. 在安装目录下(默认是C盘)  
wamp64(32)的bin目录下找到  
mysql目录进入mysql5.7.24目录    
再进入到bin目录下
复制这个路径，比如这里是  
``` C:\wamp64\bin\mysql\mysql5.7.24\bin\ ```  
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/wampmysqlbin.png)   
## 编辑PATH
1. 点击新建将复制的内容添加到新建的一行处  
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/pathedithomepage.png)   
1. 然后一路确定  
## 检验配置是否异常
1. Win + R 输入 cmd 打开命令提示符  
1. 输入 ```mysql -V ```  
显示如下则说明path路径配置完成  
![Alt text](https://github.com/CerteKim/BNG/blob/master/mysql/img/cmdmysqlv.png)   
