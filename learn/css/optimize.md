# CSS最佳实践
## 避免使用@import
CSS通过使用`@import url(CSS url)`来加载其他CSS文件。但使用@import的话，浏览器会在下载解析包含的@import的CSS后，才会在再加载@import的CSS文件。
解决方法是使用<link>标记来替代@import。因为<link>是并行加载的。

## 避免CSS表达式
css表达式只能在IE中使用。css表达式可以使用了JavaScript表达式。如：
``` css
background-color: expression((new Date()).getHours()%2?"#FFFFFF": "#000000" );
```
但是，在页面显示，缩放时，页面滚动、乃至移动鼠标时都会要重新计算css表达式的值，以致产生性能的影响。

## css选择器的优化
http://www.w3cplus.com/css/css-selector-performance

## 移除无匹配的样式
移除无匹配的样式，有两个好处：
1. 缩减样式文件的体积，加快资源下载速度
2. 对于浏览器而言，所有的样式规则的都会被解析后索引起来，即使是当前页面无匹配的规则。移除无匹配的规则，减少索引项，加快浏览器查找速度

## 参考
* [高性能CSS](http://www.alloyteam.com/2012/10/high-performance-CSS/)
* [CSS选择器的优化](http://www.w3cplus.com/css/css-selector-performance)