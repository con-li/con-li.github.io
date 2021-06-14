---
layout: post
title: "自建博客从WordPress迁移到Jekyll"
author: Cong Li
date: 2020-08-06 09:05:15
header-style: text
tags:
- 生命体验
- 商业分析
- 自建博客   
- WordPress
- Jekyll
---
自建博客之前使用WordPress框架，空间租用付费服务器资源（阿里的云虚拟主机，最低一档约300元/年）。目前转向Github Pages方案，因静态页面满足需求，且无费用。实际使用中发现静态页面访问也比较快。

### 1. Github Pages方案怎么做

Github Pages提供免费的静态页面托管服务，支持Jekyll框架。本次使用[黄玄的博客模板](https://github.com/Huxpro/huxpro.github.io)。流程如下，主要参考[BYQiu](https://www.jianshu.com/p/e68fba58f75c)、[Meswx](https://www.jianshu.com/p/3a0714c7eddf)、[西镜tristan](https://blog.csdn.net/h_meichuan/article/details/83692611)的教程。

- Github注册账户
- Github上，fork博客模板的仓库

  - 仓库改名。这里要注意命名。比如我的Github用户名是con-li，那么仓库命名为con-li.github.io
- 本地电脑，安装Github Desktop，clone上述仓库到本地

到这里，基本搭建好博客。后续维护，可本地搭建一个Jekyll框架，提高调试效率。

- 本地电脑安装ruby环境
- 在ruby环境中安装Jekyll框架，指定Jekyll框架的server地址是本地的Github仓库。
  - 调整默认路径到本地Github仓库，比如我的情况 `cd C:\Users\zone\Documents\GitHub\con-li.github.io\\_posts`
  - 在默认路径启动Jekyll服务 `jekyll server`
  - 浏览器输入localhost:4000，访问本地网页

为访问方便，可购买较简明的域名地址，再绑定到Github Pages地址。

- 修改已购买域名的cname类型解析记录。
- 进入Github Pages仓库的settings选项卡，在"GitHub Pages"的子选项栏目里，把已购买域名地址添加到Custom domain. 后续Git同步，本地仓库也会出现cname文件。

### 2. 从WordPress迁移到Jekyll

核心工作是博客内容格式的转换，把WordPress的XML格式内容，转化为Jekyll需要的Markdown格式内容。

对于内容格式转化，[Jekyll官方教程](https://jekyllrb.com/docs/migrations/)未操作成功，从一个[博客](https://www.inksay.com/the-easiest-way-convert-wordpress-posts-to-jekyll-markdown-files/)上看到用WordPress插件解决。实际操作流程如下所示。

- 远程服务器的WordPress框架安装插件"wordpress2jekyll"
- 插件使用，有一点注意，要在它的默认目录下建立名为"jekyll"的文件夹，再在其中建立名为"_ posts"、"_ assets"、"_ data"的空文件夹。

### 3. 可能用到的软件工具

- Github Desktop，操作Github Pages仓库
- FileZilla/Putty，操作购买的远程服务器