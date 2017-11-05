---
title: 移动端页面碰到的问题
date: 2017-11-05 15:16:02
tags: [前端（Front-end）,Scattered,Style]
categories: CODE
---
**去除input边框线**
如果去除下面默认样式之后还是有边框线
```{
    border:none;
    //border:none 0;
    outline:none
}```
可以试试下面这个属性
``` 
-webkit-tap-highlight-color: rgba(0, 0, 0, 0) 
```

---
&emsp;&emsp; 在ios safari浏览器里面，如果在input框的input事件中进行了js逻辑处理，*有可能*造成在点击键盘的删除时，删除最后一个时，input光标前多出一个空字符。
```
if($(this).val==""){
    $(this).parent().find('.ex').css('display','none')
}
```
`将处理逻辑写在settimeout()里面，异步执行可解决`
```
if($(this).val==""){
    settimeout(
        function(){
            $(this).parent().find('.ex').css('display','none')
        },10)
}
```






