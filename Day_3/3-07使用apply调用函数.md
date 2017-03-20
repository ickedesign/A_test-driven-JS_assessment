### 3-07使用apply调用函数

> 题目描述

实现函数 callIt，调用之后满足如下条件
1、返回的结果为调用 fn 之后的结果
2、fn 的调用参数为 callIt 的第一个参数之后的全部参数 

>输入例子:

``` js
var a = 1;
var b = 2; 
var test = function (first, second) { 
	return first === a && second === b;
}; 

callIt(test, a, b);
```

>输出例子:

true

> 实现代码：

``` js 
function callIt(fn) {
    //将arguments转化为数组后，截取第一个元素之后的所有元素
    var args = Array.prototype.slice.call(arguments,1);
    //调用fn
    var result = fn.apply(null,args);
    return result;
}

```




