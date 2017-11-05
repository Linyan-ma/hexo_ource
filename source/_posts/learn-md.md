---
title: MarkDown快速入门
date: 2017-11-03 15:01:35
tags: 
categories: CODE
---
学习使用MarkDown基础语法的使用，仅包含最基本的几个符号标识，仅为了能够快速使用MarkDown写blog。

## #号表示标题
1-6个#号代表1-6级标题
## >号表示引用
> 满纸荒唐言

## * _表示强调
单个*或者_包裹的字体会转换为<em></em>,两个包裹的字体会转换为<strong></strong>
#### 示例
>*读书人*的事，哪能叫__窃__呢

## *、+、- 无序列表
#### 示例
+ first
+ second


## \1. \2. 有序列表
#### 示例
1. 程序一
2. 程序二

## \[ 链接的名称 \](链接地址) 文字链接
  #### 示例
  [百度一下](https://baidu.com)

## ![文本内容](链接地址) 图片链接
在文字连接前加上!即可

## \`\`\`(反引号) 代码块引用
  #### 示例
```
var defferd= new defferd();
  defferd.resolve()
```
## 四个空格或者tab制表符也可表示代码块(原样输出格式化好的代码块)
#### 示例

    var promise=new promise() 
    promise.then(function(){
      console.log("running")
    })
## 加横线分割
在空白行下面加---可画一条横线

## 首行缩进
在行首添加&emsp;&emsp;