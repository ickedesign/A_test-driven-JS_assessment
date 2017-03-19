### 2-07正确的使用parseInt

> 题目描述

修改 js 代码中 parseInt 的调用方式，使之通过全部测试用例 

>输入例子

parse2Int('12'); parse2Int('12px'); parse2Int('0x12')

>输出例子

12; 12; 0

>错误代码

``` js
function parse2Int(num) {
    return parseInt(num);
}
```

> 实现代码：


``` js
function parse2Int(num) {
    return parseInt(num,10);
}
```


