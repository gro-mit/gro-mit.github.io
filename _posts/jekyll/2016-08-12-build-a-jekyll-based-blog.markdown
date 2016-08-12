---
layout: article
title:  "使用jekyll+github搭建个人博客"
date:   2016-08-12
categories: jekyll
image:
 teaser: jekyll.png
---
>##### 摘要：本文主要介绍基于jekyll和github的静态博客的搭建

---

#### 1. github的配置


##### 1.1 在github上创建github pages blog仓库

登陆github页面，点击新建repository，显示如下图，输入repository名称、描述。作为一个规范的项目，还需勾选初始化README，以便他人更好地了解你的项目。

![pic]({{ site.url }}/images/jekyll/build-a-jekyll-based-blog/shot1.png)

在建立好的repository页面打开 `Settings`，找到如下图板块，并点击 `Lunch automatic page generator`，依次点击 `Continue to layouts`、`Publish page`就可以生成相应的站点，输入对应的url即可进行访问。

![pic]({{ site.url }}/images/jekyll/build-a-jekyll-based-blog/shot2.png)

以上就完成了在github上建立repository并自动生成博客站点的任务。

##### 1.2 repository管理——引入git

在建立好站点的repository后，需要对其进行本地编辑及版本控制管理。
在linux系统(debian/ubuntu)打开terminal，输入如下代码完成git的安装：

```bash
$ sudo apt-get install git
```
当安装好git后，想要同github建立连接需要进一步进行SSH设置：

* 创建SSH Key文件，键入如下命令，并按照提示键入相应信息，即可生成`.pub`文件

```bash
$ ssh-keygen -t rsa -C "your_email@example.com"
```

* 找出`id_rsa.pub`文件，并以记事本打开，复制该文件的密钥内容。

* 登陆github，`Settings`->`SSH and GPG keys`->`New SSH key`，键入密钥内容。

* 键入如下命令，并键入`yes`查看设置结果：

```bash
$ ssh -T git@github.com
```

* 依次键入如下命令设置github用户信息：

```bash
$ git config --global user.name "your_github_username"
$ git config --global user.email "your_email@example.com"
```

经过以上SSH设置各个步骤就能让本机和github进行连接，如有问题，可以重新设置，常见的设置问题可以参考 [generating an SSH key][SSH key] 和 [SSH permission denied][SSH denied].

* 使用如下命令将远程repository同步至本地，其中`url`为该repository的url，有HTTPS和SSH两种clone方式，建议选取SSH方式以免去在clone时键入密码的环节。

```bash
$ git clone url
```

此时远程repository就被同步至本机，方便本地完善博客。

更多关于git的相关教程推荐参考[廖雪峰的git教程][git]进行学习。

#### 2. jekyll相关

关于jekyll在本机的搭建，[官方文档][jekyll doc]上有详细的说明。

##### 2.1 jekyll依赖环境

在安装jekyll前，为确保其正常运行，需要安装一些依赖环境。为此，特引用jekyll官方依赖说明如下：

> 
>    Installing Jekyll is easy and straight-forward, but there are a few requirements you’ll need to make sure your system has before you start.
> 
> * [Ruby][ruby] (including development headers, v1.9.3 or above for Jekyll 2 and v2 or above for Jekyll 3)
> * [RubyGems][gem]
> * Linux, Unix, or Mac OS X
> * [NodeJS][nodejs], or another JavaScript runtime (Jekyll 2 and earlier, for CoffeeScript support).
> * [Python 2.7][python] (for Jekyll 2 and earlier)
> 

##### 2.2 jekyll安装与使用

在安装好以上依赖后，可以通过rubygem方便地安装jekyll，并通过`-v`查看jekyll版本号以确定安装成功：

```bash
$ gem install jekyll
$ jekyll -v
```

之后就可以使用jekyll新建博客：

```bash
$ jekyll new myblog
$ cd myblog
myblog $ bundle install
myblog $ bundle exec jekyll serve
# initialize jekyll blog
```

以上就在本机完成了一个基于jekyll的简单博客站点，之后可以对该站点进行个性化，在每次更新修改后可以键入如下命令打开本机服务：

```bash
$ jekyll serve
#  browse to url http://localhost:4000
```

在浏览器中访问如上url，显示如下：

![pic]({{ site.url }}/images/jekyll/build-a-jekyll-based-blog/shot3.png)

##### 2.3 jekyll搬家

现在将之前clone到本机的repository文件夹内的非隐藏除README文件的其他文件删除，并将在本机搭建好的站点文件夹内的所有文件复制到repository文件夹内，使用git将其push到github上，就可以通过github网址访问博客了。



[SSH key]: https://help.github.com/articles/generating-an-ssh-key/
[SSH denied]: https://help.github.com/articles/error-permission-denied-publickey/
[git]: http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000 
[jekyll doc]: https://jekyllrb.com/docs/home/
[ruby]: https://www.ruby-lang.org/en/downloads/
[gem]: https://rubygems.org/pages/download
[nodejs]: https://nodejs.org/en/download/
[python]: https://www.python.org/downloads/
