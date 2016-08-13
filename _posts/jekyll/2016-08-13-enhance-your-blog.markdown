---
layout: article
title:  "为博客添加google analytics访问统计和disqus文章评论功能"
date:   2016-08-13
categories: jekyll
image:
 teaser: jekyll.png
---
>##### 摘要：本文主要介绍基于google analytics的博客访问统计和基于disqus的文章评论功能

---

#### 1. google analytics

[google analytics][analytics]是google提供的站点访问情况统计，登陆google账户，创建新的analytics账户如下图所示：

![pic]({{ site.url }}/images/jekyll/201608/shot5.png)

填写账户名称以及你的博客名称和url等信息，点击`获取跟踪ID`得到如下代码段：

```javascript
<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

  ga('create', '这里是你的跟踪id', 'auto');
  ga('send', 'pageview');

</script> 
```

将其粘贴到`_layouts`->`default.html`中的`</head>`标签以上就可以了。但更推荐的做法是在`_include`文件夹新建`analytics.html`文件讲该段代码粘贴其中，在`_layouts`->`default.html`文件同样的位置加入{% raw %}`{% include analytics.html%}`{% endraw %}标记，方便管理。

以上就完成了访问统计的功能嵌入，经过一段时间即可查看博客访问情况。


#### 2. disqus

disqus博文评论功能添加和analytics类似。首先，需要在[disqus][disqus]上注册账户并邮箱验证。

![pic]({{ site.url }}/images/jekyll/201608/shot6.png)

如图选择`install Disqus`并按照提示输入博客信息，之后选择`Universal Code`，如下图所示：

![pic]({{ site.url }}/images/jekyll/201608/shot7.png)

复制代码段到`_layouts`中你的博文模板文件`</article>`与`</div>`标签之间。在博文下方就会出现disqus社交评论功能界面。同样地，可以按照google analytics推荐的方法嵌入代码段。

![pic]({{ site.url }}/images/jekyll/201608/shot8.png)

以上就完成了社交评论的引入，需要说明的是，disqus支持disqus、facebook、twitter和google账号(注：非vpn下disqus评论模块无法显示)，为了使用微博、微信等国内的账号登陆，可以使用[友言][youyan]、[多说][duoshuo]和[搜狐畅言][changyan]等社会化评论工具。

注：其实SKINNY BONES主题已内嵌了disqus功能，如需开启，操作如下：

![pic]({{ site.url }}/images/jekyll/201608/shot9.png)



[analytics]: https://analytics.google.com
[disqus]: https://disqus.com/
[youyan]: http://www.uyan.cc/
[duoshuo]: http://duoshuo.com/
[changyan]: http://changyan.kuaizhan.com/
