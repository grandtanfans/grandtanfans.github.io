---
layout: post
title: 'Hello World'
date: 2019-12-26
author: 痰黄刀
color: rgb(255,210,32)
cover: 'https://s2.ax1x.com/2019/12/26/lA0L24.jpg'
tags: 博客系统
---

> 测试文本：引言内容。

目录：

* TOC
{:toc}

本帖无实质性更新。主要是为了博主本人熟悉和该博客相关的一些内容和配置，为之后的发文提供便利。

注意：封面图片似乎不会完全显示，但具体显示到什么程度，也还需要再看一下。<br/>注意封面头部托管到网上加载速度会略快一些。<br/>正文图片测试（同封面图片）：

![lA0L24.jpg](https://s2.ax1x.com/2019/12/26/lA0L24.jpg)

这个是可以正常显示的。

关于标签的配置：在头部直接按照这个格式写 `tag: tag1 [tag2 tag3 ...]` 即可，标签之间不需要加逗号，也不需要在标签集合的两边加上方括号之类的。

# 一级标题

## 二级标题

### 三级标题

This site aims to be a comprehensive guide to Jekyll. We’ll cover topics such as getting your site up and running, creating and managing your content, customizing the way your site works and looks, deploying to various environments, and give you some advice on participating in the future development of Jekyll itself.

### So what is Jekyll, exactly?Permalink

Jekyll is a simple, blog-aware, static site generator. It takes a template directory containing raw text files in various formats, runs it through a converter (like [Markdown](https://daringfireball.net/projects/markdown/)) and our [Liquid](https://github.com/Shopify/liquid/wiki) renderer, and spits out a complete, ready-to-publish static website suitable for serving with your favorite web server. Jekyll also happens to be the engine behind GitHub Pages, which means you can use Jekyll to host your project’s page, blog, or website from GitHub’s servers for free.

### Helpful HintsPermalink

Throughout this guide there are a number of small-but-handy pieces of information that can make using Jekyll easier, more interesting, and less hazardous. Here’s what to look out for.

### 代码高亮

Jekyll 使用 [Rouge](http://rouge.jneen.net) 这个使用 Ruby 编写的代码高亮器来实现代码的高亮，Rouge 在 Jekyll 3 及以上的环境可用（这年头应该没有憨比还在用 Jekyll 2 吧）。

代码高亮示例如下：

<pre>
{% highlight objective_c %}
NSArray *backup = @[@"苏", @"米", @"珂", @"瓜"];
// 可能有语法错误，我只是拿这玩意儿举个例子。
for (id obj in backup) {
    NSLog(obj);
}
{% endhighlight %}
</pre>

实装结果：

{% highlight objective_c %}
NSArray *backup = @[@"苏", @"米", @"珂", @"瓜"];
// 可能有语法错误，我只是拿这玩意儿举个例子。
for (id obj in backup) {
    NSLog(obj);
}
{% endhighlight %}

上面示例里代码块的头部 `{% highlight objective_c %}` 中 `objective_c` 那个就是语言的标识符。关于 [Rouge](http://rouge.jneen.net) 所支持的语言的标识符，上这里去看：[Rouge wiki](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers)；Jekyll 基于 Rouge 的语法高亮，可以参考这个：[Syntax Highlighting in Jekyll](http://sangsoonam.github.io/2019/01/20/syntax-highlighting-in-jekyll.html)。

不过一般来说，你描述 TB 博客也没必要用到代码高亮的文学手法，除非是你整个赛博朋克的文风。。。

### 评论功能

用的 [来必力](http://livere.com/)。配置很简单，都不要求能看懂英语啥的。这个东西配完一次基本上不需要配第二次，只是说下当前部落格的评论功能是用的 **来必力** 而已。

### 视频测试

如果是使用 [`<iframe>` 标签](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe) 的话，搬 YT 的视频需要 `iframe[src]` 的值为 `协议://域名/embed/视频id` 的形式。我们也将会用 `<iframe>` 这种手法：

<iframe type="text/html" width="100%" height="385" src="https://www.youtube.com/embed/VHRDPSOAC0A" frameborder="0"></iframe>

上面的视频信息：<br/>来源：<br/>YouTube：<br/>Up 主：[就等死再不運動](https://www.youtube.com/user/jkg8954200)<br/>视频链接：[DOUYU 蘇恩 pk 米儿 20191016](https://www.youtube.com/watch?v=VHRDPSOAC0A)

如果使用 [`<video>` 标签](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)，以现有的资源配置无法实现视频的播放，必须另外购买视频服务器或是购买专业视频托管服务。有这个钱还不如直接给老痰刷超火。