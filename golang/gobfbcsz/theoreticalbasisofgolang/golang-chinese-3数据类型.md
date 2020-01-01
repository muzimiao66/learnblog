# 三、词法与数据类型

## 3.2数据类型
### 3.1.6 表达式
－表达式带代表了把操作符和函数作用于操作数的计算方法。
### 3.2.3  切片
```golang
//slice1 初始化原值
slice1 = []string{"go","python","java","C","Ruby","Erlang"};
//再次对变量slice1的值进行扩展
slice1 = append(slice1,"Lisp");
```
  这时将会有一个新的数组值被创建并并初始化。这个新的数组值将作为append函数新创建
的切片值的底层数组，并包含原切片值中的全部元素值以及作为扩展内容的所有元素值。
 

内建函数append的第二个参数是一个可变长参数，append 函数把两个元素类型相同的切片值连接起来。例如：
```golang
slice1 = append(slice2,slice1...);
var slice4 = []string
slice4 = append(slice4,slice1);
```
