# 第三题

## 前请概要

### 关系运算符
假设 a = 10; b = 20
| 运算符 | 说明 | 举例 |
| ------ | ---- | ---- |
| -eq | 左右数字是否相等 | ```$a -eq $b``` 返回 false |
| -ne | 左右数字是否不等 | ```$a -ne $b``` 返回 true |
| -gt | 左数是否大于右数 | ```$a -gt $b``` 返回 false |
| -lt | 左数是否小于右数 | ```$a -lt $b``` 返回 true |
| -ge | 左数是否大于等于右数 | ```$a -ge $b``` 返回 false |
| -le | 左数是否小于等于右数 | ```$a -le $b``` 返回 true |

### for 循环
例子3：
```shell
for (( i=1;i<10;i++ ))
do
    commandN
done
```

### while 循环
例子4：
```shell
i=1
while ["$i" -ne 10]
do
    commandN
    ((i++))
done
```

## 题目
写不出来可以直接放弃

请使用 Shell 编写一个输出一个 方形 9x9 乘法表

tips:

1. ```echo```输出默认换行

1. 只打一个```echo```直接换行

1. ```echo -n```输出不换行

1. ```echo -e```启用转义字符  
例如：  
```echo -e 你"\t"我"\t"他"``` = ```printf("你\t我\t他");```

1. 所以你们大概会用到
```echo -ne```