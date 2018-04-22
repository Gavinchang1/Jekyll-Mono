---
layout: post
title: HTML标签--<head>
author: 常鑫同学`
---

&nbsp;&nbsp;脸肯定是不想打的，又确实懒，只有捡软柿子捏咯，群里面各个都是人才，群主小姐姐说话又那么好听，超喜欢的。

&nbsp;&nbsp;这篇文章真的只讲`<head>`,`<head>`里面的东西以后再说 :joy:。

`<head>`标签，作为一个容器，主要存放网页描述和外部资源引用等信息，基本上全是给浏览器看的。MDN关于`<head>`的描述如下
>HTML head 元素 规定文档相关的通用信息（元数据），包括文档的标题，文档的样式和脚本的链接（定义）等。

先说兼容性：没有不支持的浏览器，这都不支持还怎么在浏览器圈混 :unamused:

`<head></head>`中`<title>`是唯一必须元素，确定文档标题，应该是`<head>`中唯一可见的元素。`<meta>`,元数据，描述网页信息，这位大佬神通广大，尤其是在SEO和移动端适配方面，下次详谈。`<link>`引入外部资源，通常用于引入外部CSS文件，但事情没有这么简单（推眼镜），第三篇写它 :smile:。`<base>`预设url路径，但只对相对路径有效；`<style>`引入css样式；`<script>`引用或者嵌入可用脚本，基本为js;`<noscript>`用于在脚本未执行的情况下作出反应。第四篇写剩下的这些。:smile:
就拿emmet的默认模板作为示例吧，毕竟一篇技术文章，没点代码也说不过去（摊手）
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

不过不写`<head>`好像也可以，浏览器都会自动创建一个`<head>`。
```
<!DOCTYPE html>
<html lang="en">
<body> 
</body>
</html>

```

![firefox](https://github.com/Gavinchang1/gavinchang1.github.io/blob/master/images/firefox.jpg)


![chrome](https://github.com/Gavinchang1/gavinchang1.github.io/blob/master/images/chrome.jpg)


<a href="http://www.stevesouders.com/blog/2010/05/12/autohead-my-first-browserscope-user-test/">当然，不是所有浏览器都可以。</a>

哦，对了，它以前有个全局属性`<profile>`，规定文档url的一系列规则，H5中删了。其他剩下的东西就看MDN这张表吧。
![MDN](https://github.com/Gavinchang1/gavinchang1.github.io/blob/master/images/MDN.jpg) 

P.S.这篇文章先试试水，以后尽量不这么水。

>参考文献：<a href="https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/head">MDN文档
