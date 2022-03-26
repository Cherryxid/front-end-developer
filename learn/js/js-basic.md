## 标识符    

> 标识符（identifier）是用来识别具体对象的一个名称。常见的标识符就是变量名和函数名。

标识符命名规则    

1. 第一个字符可以是任意Unicode字母，以及美元符号（$）和下划线（_）
1. 第二个字符及后面的字符，还可以用数字。
1. JavaScript有一些保留字，不能用作标识符：arguments、break、case、catch、class、const、continue、debugger、default、delete、do、else、enum、eval、export、extends、false、finally、for、function、if、implements、import、in、instanceof、interface、let、new、null、package、private、protected、public、return、static、super、switch、this、throw、true、try、typeof、var、void、while、with、yield。

## 数据类型
见http://javascript.ruanyifeng.com/grammar/basic.html 的数据类型

## 变量定义
加不加var的区别

## 操作符
+,-,*,/,++,--,

## js中的为true和false的值
为false的值
```
false
null
undefined
0
''// 空字符串
obj.undefinedProperty
```
其他值均为true。
注意：
```
[] == false // -> true, [] not falsy though
```
## `==`与`===`的区别
用`==`对两个值进行判定时，会进行类型转化，而`===`不会,如：
```
1 == '1'// true
1 === '1' // falsse
```
## 继承
### 原型链
## 闭包
## javascript 怪异的地方