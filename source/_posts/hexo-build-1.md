---
title: 基于hexo框架搭建个人博客
date: 2020-09-28 13:43:35
tags:
---
### 什么是 Hexo？
Hexo 是一个快速、简洁且高效的博客框架。Hexo 使用 Markdown（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。


### 基于Hexo搭建个人博客准备
需要提前准备好nodejs，git，hexo等。

### Git简介以及安装

Git:分布式版本控制系统。如果相对Git有更多的了解，可以去看看[廖雪峰老师对Git的简介](https://www.liaoxuefeng.com/wiki/896043488029600/896067008724000)

Git的作用：多人协作，版本控制

Git的安装：

1. 下载Git，[Git下载地址](https://git-scm.com/download/win)
2. 安装就一路next即可。
3. 安装完成以后，需要配置自己的信息，打开Git控制台，右键找到Git Bash Here

```
    git config --global user.name "你的昵称"
    git config --global user.email 你的邮箱
```

到此，Git环境就已经准备好了

### NodeJs环境准备
NodeJs的下载安装教程
1. 到[NodeJs中文下载地址](http://nodejs.cn/download/) 进行下载，Windows系统选择windows的.msi文件下载，linux系统选择x64 64位下载。
<code>(Node.js 版本需不低于 10.13，建议使用 Node.js 12.0 及以上版本，版本太低后续下载Hexo的时候会报错)</code>
2. 下载完成以后，安装也是一路next即可。
3. 判断NodeJs环境是否成功, 打开Git控制台

```
    node -v;
    npm -v;
```
4. 出现相应的版本即安装成功。

### Hex框架
所有必备的应用程序安装完成后，即可使用 npm 安装 Hexo。
```
$ npm install -g hexo-cli
```

### 本地初始化项目并启动

1. 建立一个空的文件夹存放博客。
2. 在文件夹内打开Git控制台,执行以下命令
```
hexo init
npm install
```
<code>如果npm下载东西很慢的话，可以走国内的淘宝镜像，具体方法：[使用教程](https://www.cnblogs.com/haozehua/p/10523690.html)</code>

3. 本地启动项目
```
    hexo s
```
4. 验证本地项目是否搭建成功,打开浏览器访问http://localhost:4000/，如果出现博客页面即搭建成功
