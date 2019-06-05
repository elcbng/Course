# 简单的数据库操作  
- 作者Cerbur
## 欢迎界面以及执行语句
```sql
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 3
Server version: 5.7.24 MySQL Community Server (GPL)

Copyright (c) 2000, 2018, Oracle and/or its affiliates. All rights reserved.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql>
```
每次登录 MySQL 后都会有这个界面  
``` mysql> ```之后都是执行 MySQL 的语句  
直到遇到 ``` ; ``` 分号结束该语句  
每行 enter 如果没分号将会换行  
有分号则执行分号前的语句
```sql
mysql> SHOW
    -> DATABASES
    -> 
    -> ;
```
举个例子  
上面则是未遇到分号后一直换行  
MySQL 执行的时候会自动合并起来  
所以我们写 MySQL 语句的时候  
可以为了方便查阅换行写  
```
一点小贴士：
所以执行的代码可以先在文本编辑器上完成后  
复制到 MySQL 中执行这样有利于后期修改  
但千万要注意字符集这里一律使用 utf-8 字符集  
文本编辑器推荐使用 Visual Studio Code
```
- 好啦我们开始讲执行语句吧  
## 显示所有数据库
```sql
SHOW DATABASES;
show databases;
```
>MySQL 关键字大小写不敏感  
所以以上两种方式都是正确的  
个人习惯会喜欢关键字用大写  
>
这个语句将显示 MySQL 内所存着的所有数据库  
执行语句显示出结果后显示~~执行的结果集~~的数量和时间(找不到适合的话说)  
执行结果:
```sql
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| db_shop            |
| db_weibo           |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
6 rows in set (0.00 sec)
```
## 创建数据库
- 语法结构
```sql
CREATE DATABASE `[database's name]`;
```
>```[database's name]```中填入数据库名字  
开头可以是英文、下划线、中文(但不推荐)  
不能是数字、特殊字符等  
有个比较推荐的命名```db_[name]```  
db为database的缩写，后面下划线加名称  
``` ` ` ```这个小点号可省略但不推荐  
有些特殊情况可能会将空格当作是名字的一部分  
用``` ` ` ```将内容套入其中可以避免一些出乎意料的意外  
- 举个例子
```sql
CREATE DATABASE `db_book`;
```
执行结果:
```sql
mysql> CREATE DATABASE `db_book`;
Query OK, 1 row affected (0.00 sec)
```
这样我们是看不到到底创建了什么的  
所以这时候要执行上一次的语句  
查询数据库
```sql
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| db_book            |
| db_shop            |
| db_weibo           |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
7 rows in set (0.00 sec)
```
可以看到 ``` db_book ``` 被创建了  

## 使用数据库  
- 语法结构
```sql
USE `[database's name]`;
```
执行后可以理解为进入了一个新的目录中  
可以在这个目录中操作对应的表(TABLE)  
- 举个例子   
```sql
USE `db_book`;
```
执行结果:
```sql
mysql> USE `db_book`;
Database changed
```
## 删除数据库  
- 语法结构
```sql
DROP DATABASE `[database's name]`;
```
 ``` DROP DATABASE + 数据库名```   
执行完后即可~~跑路~~  
这是 MySQL 最好玩的语句  
遇事不决 删库跑路  

- 举个例子
```sql
DROP DATABASE `db_book`;
```
执行结果:
```sql
mysql> DROP DATABASE `db_book`;
Query OK, 0 rows affected (0.00 sec)
```
好哒让我们再来查看所有数据库吧
```sql
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| db_shop            |
| db_weibo           |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
6 rows in set (0.00 sec)
```
好哒可以看到 ```db_book ``` 已经成功被我们删掉咯  
- 好好温习下本节内容  
- 删库跑路只是个玩笑  
- 真的出了大事情可是有法律责任的  
- 多敲一下  
- 实在不行复制粘贴吧  
- 然后对比自己是不是哪里语句出现了问题  
- 比如database少了s或者是多了s