# 2019年电子科技协会网络组招新笔试
### **姓名：**  
*预计最短答题时间：30 分钟*，**每道题目都给出了一些阅读材料或提示，不会的题目大胆猜测**  

## 一、boom
使用 C 语言编写一个名为`boom`的函数，使该函数被调用时输出大量乱码并使程序崩溃。常见的导致程序崩溃的原因包括但不限于内存越界访问、栈溢出。
```
void boom()
{
    



}
```
---
## 二、input
使用 C 语言编写一个函数，检查输入的字符串是否超过所给字符数组所能容纳的上限，如果超过则调用上一题的 `boom` 函数，否则将字符串存入字符数组 s 并返回。使用`scanf("%c",&c)`可以每次只读取一个字符。由于给定的字符串长度可能非常长，所以通过定义一个非常大的字符数组一次性读取整个字符串是不可以的。
```
void input(char s[])
{
    char c;
    int s_length, i;







    return;
}
```
---
## 三、html 与 css

css 全称 Cascading Style Sheets，可以理解为是一种用于修饰 html 的语言，html 由形似 `<name></name>` 的标签组成，标签内包含该标签的名称与其他信息，标签名可以重复。下面的两个例子在**效果上是相同的**。
```
把 style 写在 <></> 标签内：

<div style="length: 100%; width: 100%; top: 10%;"></div>
<div style="length: 100%; width: 100%;"></div>
<p   style="length:  50%; width: 100%;"></p>
```
```
把 style 单独写，相同的内容可以使用逗号分隔的方式一起定义，特别的内容仍然写在原来的标签里：

<div style="top: 10%;"></div>
<div></div>
<p></p>

<style>
div{
    length: 100%;
}
p{
    length: 50%;
}
div, p{
    width: 100%;
}
</style>
```

通过分析上面的例子，简要描述当标签数量增大时，`把 style 单独写`的方式有什么优点，又有什么缺点。
```






```
---

## 四、shell

### 阅读材料

Shell 是命令行，也可以编程。例如，下面这段代码是可以使用 shell 执行的：
```
echo 准备好开始循环了吗!
echo "#!/bin/bash" >> run.sh
chmod +x run.sh
echo "echo 循环中" >> run.sh
echo "bash run.sh" >> run.sh
bash run.sh
```
运行的结果是生成一个包含 shell 代码的文件并执行文件中的代码。

#### echo
以下是一个输出：```Hello World!```的 Shell 程序代码：
```shell
echo "Hello World!"
```

执行结果：
```shell
Hello World!
```

#### 输入/输出重定向
| 命令 | 说明 |
| ---- | ---- |
| `命令 > 文件` | 输出重定向到文件，不保留文件原有内容 |
| `命令 < 文件` | 输入重定向到文件 |
| `命令 >> 文件` | 输出重定向到文件尾，保留文件原有内容 |

#### 基本文件操作
复制 file1 到 file2
```bash
cp file1 file2
```

删除
```bash
rm file
```

移动
```bash
mv file1 file2
```

输出文件夹中所有文件的名字
```bash
ls
```
执行结果：
```
桌面
文档
视频
照片
用户
网络组招新笔试题目.docx
```

### 题目
请编写一个 Shell 脚本，将 `我的文件夹下面有：` 和 **当前目录下所有文件名字** 输出到指定的文件，文件名随意

```
在此处填写答案：

```

**命令执行的结果应当是生成一个文本文件，文件内容类似：**
我的目录.txt：
```
我的文件夹下面有：
bin
home
dev
etc
system
```
---
## 五、Java
在 Java 的类中，包含着**变量、方法**。使用 private 修饰时，类中的**变量、方法** 不能被类外部的代码访问，而使用 public 修饰时则可以。我们可以通过编写一个 public 修饰的方法来获取一个 private 修饰的值。在类内部可以通过 this 访问其他成员，例如 this.thing 特指当前类中名为 thing 的成员变量。  
**补全 成员方法2 实现通过该方法获取 age 的值**
```java
//这是一个名为Person的类，类似C的结构体，与C不同的是，类中可以带方法(C中叫函数)
public class Person {

    //这是一个私有成员变量
    private int age;
    //这是一个公有成员变量
    public String name;

    //这是一个公有成员方法1
    public void setAge(int age) {
        this.age = age;
    }
    //这是一个公有成员方法2
    public int getAge() {
        /*补充你的代码*/
        _______________________
    }
}

    Person person = new Person();
    String name = person.name; //name用public修饰所以可以访问 
(!) int age = person.age; //age用private修饰所以不能访问;
    int age = person.getAge(); //getAge()用public修饰所以可以访问
```