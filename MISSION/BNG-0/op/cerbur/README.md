1. (以下内容结合下方代码一同理解)众所周知**Java**是世界上最好的语言，在Java的类中，包含着**变量、“函数”**。当我们使用private修饰变量或者函数时，类中的**变量、“函数”** 将不能被访问，而使用public修饰时则可以。所以我们可以通过编写一个public的“函数”来获取private修饰的这个值。而在内部可以通过this来访问，例如this.thing特指名为thing的成员变量，即可获取thing的值。**那么现在外部无法访问成员变量，请补全通过 成员方法2 来获取成员变量的值**
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
    //int age = person.age; //age用private修饰所以不能访问;
    int age = person.getAge(); //getAge()用public修饰所以可以访问，请补全getAge()
```
---
2. 电子科技协会有着许多部门、每个部门有着许多成员，每个成员又有着不同的职位。现在我们设计了如下这样一些表格来存协会成员的信息。    

①存有什么部门的表格

|部门id|部门|  
|:----:|:----:|  
|1|网络组|  
|2|主席团|
|3|网宣部|
|4|项目部|  
②存有什么成员的表格

|成员id|成员名称|  
|:----:|:----:|  
|1|Cerbur|  
|2|子曦|
|3|木舟|
|4|鱼饼|   
③存成员与部门关系的表格
|成员id|部门id|  
|:----:|:----:|  
|1|1|  
|2|1|
|3|3|
|4|2|   
请试者写出，在广东工业大学里，存学院、专业的3个表格。