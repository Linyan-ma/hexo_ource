---
title: 计算base64图片大小
date: 2017-12-21 15:54:39
tags:
---
## Base64图片编码原理：
> Base64编码要求把3个8位字节（3*8=24）转化为4个6位的字节（4*6=24），之后在6位的前面补两个0，形成8位一个字节的形式。 如果剩下的字符不足3个字节，则用0填充，输出字符使用’=’，因此编码后输出的文本末尾可能会出现1或2个’=’

## JS实现代码
```  function getBase64FileByte(str) {
            str = str.substring(22);
            var equalIndex = str.indexOf('=');
            if (str.indexOf('=') > 0) {
                str = str.substring(0, equalIndex);
            }
            var strLength=str.length;
            var fileLength=parseInt(strLength-(strLength/8)*2); 
            return fileLength;
        }
```