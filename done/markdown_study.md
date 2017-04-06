# Markdown 学习笔记
<span id="top"></span>
[测试url跳转][end] 
##目录结构
<!-- MarkdownTOC -->

- [MD语法](#md语法)
- [MD 增加目录功能](#md-增加目录功能)
- [MD 其他的一些技巧](#md-其他的一些技巧)
  - [对色彩的支持](#对色彩的支持)
  - [页面内的跳转](#页面内的跳转)

<!-- /MarkdownTOC -->

<a name="md语法"></a>
# MD语法

>  * [中文版官方教程][tutorial]
>  * [网友详细解析的教程][good]

[返回目录](#top)  

<a name="md-增加目录功能"></a>
# MD 增加目录功能   
>  MD 中增加目录有以下几种方法
> >  1. 一种的利用MD 页面跳转语法，手工制作。这个可以参考sublime 中各个插件包中的README.md，  
> >   是一个很好的示例。  
> >  2. 第二种是利用插件(MarkdownTOC)来完成. [这个最好参考官方教程][office],只要在用户配置里增加以下几项就可以
> >  ![md_toc_config](../../images/md_toc_config.png)   
> >  需要特别注意的就是"default_bracket",我用ST是选的Github的配色，所以只有这个起作用。  
> >   ![md_toc_config](../../images/md_toc_tip.png)   

[返回目录](#top)
<a name="md-其他的一些技巧"></a>
# MD 其他的一些技巧    
<a name="对色彩的支持"></a>
## 对色彩的支持   
> 在网上翻阅的不少，貌似只有[<font color="red" size=12 face="STCAIYUN">这种方法</font>][color]. 感觉还行，大家可以试试看。

<a name="页面内的跳转"></a>
## 页面内的跳转
>  页面跳转其实也就是利用锚点的功能，当定义完id后，有两种方式，一种直接利用MD的跳转语法\[](#id),  
>  另一种是使用MD的url语法，在文章开头有个测试样例，跳转到底部的。具体在MD中定义如下：

```   html

 这个id放置在你想要跳转的地方
<span id="mid" ></span> 

1. url方式的使用
[mid][mid] 
[mid]: #mid   

2. 跳转语法的使用
[mid](#mid)

```

[返回目录](#top)  

***
<font color="gray" size=5.8  style="font-weight:bold;">感谢文中各个链接作者的贡献</font>    

<span id="end" ></span>

[tutorial]: http://wowubuntu.com/markdown/index.html
[good]: http://www.cnblogs.com/tianjintou/p/4572386.html#_labelTop
[office]: https://packagecontrol.io/packages/MarkdownTOC
[end]: #end 
[color]: http://blog.csdn.net/testcs_dn/article/details/45719357/
