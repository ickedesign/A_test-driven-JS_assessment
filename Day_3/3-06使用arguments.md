### 3-06使用arguments

> 题目描述

函数 useArguments 可以接收 1 个及以上的参数。请实现函数 useArguments，返回所有调用参数相加后的结果。本题的测试参数全部为 Number 类型，不需考虑参数转换

>输入例子:

``` js
useArguments(1, 2, 3, 4)

```

>输出例子:

10

> 实现代码：

``` js 

function useArguments() {
	var sum = 0;
    for (var i = 0;i < arguments.length; i++){
        sum += arguments[i];
    }
    return sum;
}

```




