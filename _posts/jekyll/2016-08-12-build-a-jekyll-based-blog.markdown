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

登陆github页面，点击新建repository，显示如下图，输入repository名称(以`username.github.io`的格式，这也就是你站点的url)、描述。作为一个规范的项目，还需勾选初始化README，以便他人更好地了解你的项目。

![pic]({{ site.url }}/images/jekyll/201608/shot1.png)

在建立好的repository页面打开 `Settings`，找到如下图板块，并点击 `Lunch automatic page generator`，依次点击 `Continue to layouts`、`Publish page`就可以生成相应的站点，输入对应的url即可进行访问。

![pic]({{ site.url }}/images/jekyll/201608/shot2.png)

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

在浏览器中访问如上url，显示如下就证明本地jekyll站点搭建成功：

![pic]({{ site.url }}/images/jekyll/201608/shot3.png)

##### 2.3 jekyll站点目录结构与相关设置

jekyll的站点的目录结构如下：

```bssh
.
├── _config.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.textile
|   └── on-simplicity-in-technology.markdown
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.textile
|   └── 2009-04-26-barcamp-boston-4-roundup.textile
├── _data
|   └── members.yml
├── _site
├── .jekyll-metadata
└── index.html
└── images
```

|文件(夹)|说明|
|:---:|---|
|`_config.yml`|存储站点的配置信息，可修改博客title等信息。|
|`_drafts`|用于保存未发布的博文，非必选|
|`_includes`|约等于“头文件”，在该文件夹保存的文件可被{% raw %}`{% include filename.ext %}`{% endraw %}标记形式引用在博文或者页面中。|
|`_layouts`|模板文件，例如博文及博文目录的板式等。|
|`_posts`|用于保存博文，文件命名规则依照`YYYY-MM-DD-title.markdown`，使用markdown撰写正文之前需要在文件中参照YAML格式设定头信息，如图所示：![pic]({{ site.url }}/images/jekyll/201608/shot4.png) |
|`_data`|用于保存特定形式的站点数据。|
|`_site`|可以理解为存放jekyll在站点修改更新后“编译”的文件|
|`images`|存放站点的资源文件如图片等，非必选。|
|其它|`css`文件夹存放css样式；`favicon.ico`存放于根目录，是站点在浏览器tab页的图标，可以使用`.png`或`.jpg`文件修改扩展名得到。|

##### 2.4 jekyll主题

jekyll的博客主题有很多，下面是较常用的主题网站：

* [github.com/jekyll/jekyll/wiki][theme 1]

* [jekyllthemes.org][theme 2]

* [themes.jekyllrc.org][theme 3]

在选好喜欢的主题后，可以选择将该主题的`.zip`文件下载，或者从github上将其clone下来，并将其根目录中的非隐藏文件全部替换到自己的的博客根目录中(隐藏文件是主题的git信息，需要忽略)，进行个性化设置,并执行如下命令查看模板：

```bash
$ bundle install
$ bundle exec jekyll serve
```

如果仅通过`jekyll serve`启动服务则会报错，因为模板通过bundle安装独立的依赖环境，在以后的个性化修改环节中择可以使用`jekyll serve`启动服务。

##### 2.5 jekyll搬家

现在将之前clone到本机的repository文件夹内的非隐藏除README文件的其他文件删除，并将在本机搭建好的站点文件夹内的所有文件复制到repository文件夹内，使用git将其push到github上，就可以通过github网址访问博客了。

#### 3 后记
以上就初步地完成了基于jekyll和github的博客搭建。这里需要说明的是，对于目录中结构的相关设定，可以去jekyll官网查看英文文档。也可以自己尝试修改，查看相关变化慢慢摸索jekyll的各部分功能。我所使用的博客模板源于[SKINNY BONES][skinny bones]。里面的较为详细的主题安装以及个性化设置的说明，有助于更好地了解jekyll。现在我们就可以开始在本机写博客了，之后提交到github上就完成了博客更新。



[SSH key]: https://help.github.com/articles/generating-an-ssh-key/
[SSH denied]: https://help.github.com/articles/error-permission-denied-publickey/
[git]: http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000 
[jekyll doc]: https://jekyllrb.com/docs/home/
[ruby]: https://www.ruby-lang.org/en/downloads/
[gem]: https://rubygems.org/pages/download
[nodejs]: https://nodejs.org/en/download/
[python]: https://www.python.org/downloads/
[theme 1]: https://github.com/jekyll/jekyll/wiki
[theme 2]: http://jekyllthemes.org/
[theme 3]: http://themes.jekyllrc.org/
[skinny bones]: https://mmistakes.github.io/skinny-bones-jekyll/
