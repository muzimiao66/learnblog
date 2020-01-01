# 三、词法与数据类型

## 3.2数据类型

### 3.2.3  切片
```golang
//slice1 初始化原值
slice1 = []string{"go","python","java","C","Ruby","Erlang"};
//再次对变量slice1的值进行扩展
slice1 = append(slice1,"Lisp");
```
  这时将会有一个新的数组值被创建并并初始化。这个新的数组值将作为append函数新创建
的切片值的底层数组，并包含原切片值中的全部元素值以及作为扩展内容的所有元素值。
 


