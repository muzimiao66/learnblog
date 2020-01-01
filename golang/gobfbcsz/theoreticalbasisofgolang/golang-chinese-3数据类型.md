# 三、词法与数据类型

## 3.2数据类型
### 3.1.6 表达式
&emsp;&emsp;表达式带代表了把操作符和函数作用于操作数的计算方法。

>1.基本表达式
>>- 使用操作数来表示基本表达式。[]int{1,2,3,4,5}[2]
>>- 类型转换表达式。int(v1)+v2
>>- 内建函数调用表达式。len(v3)
>>- 一个基本表达式和选择符号组成。x.f
>>- 索引表达式。[]int{1,2,3,4,5}[2]
>>- 切片符号表达式。[]int{1,2,3,4,5}[1:4]取出了切片[]int{1,2,3,4,5}的第二个到第四
个元素
>>- 类型判断表达式。interface{}(num).(int)
>>- 调用符号表达式。os.Open("/etc/profile")
### 3.2.3  切片
```golang
//slice1 初始化原值
slice1 = []string{"go","python","java","C","Ruby","Erlang"};
//再次对变量slice1的值进行扩展
slice1 = append(slice1,"Lisp");
```
&emsp;&emsp;这时将会有一个新的数组值被创建并并初始化。这个新的数组值将作为append函数新创建
的切片值的底层数组，并包含原切片值中的全部元素值以及作为扩展内容的所有元素值。
 

&emsp;&emsp;内建函数append的第二个参数是一个可变长参数，append 函数把两个元素类型相同的切片值连接起来。例如：
```golang
slice1 = append(slice2,slice1...);
var slice4 = []string
slice4 = append(slice4,slice1);
```
