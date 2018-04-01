---
layout: post
title: "搭建个人博客hexo+github详细完整步骤"
date: 2016-12-20 14:48
comments: true
tags: 
	- hexo
	- 博客
---
参考了别人的一些方法，在总结了自己的安装部署过程。把完整步骤分享给大家，如果我的步骤不行，大家可以参考其他人的（有用过Git、node、GitHub的应该可以很快搞定，没用过的可能要花费点时间！）


```angular2html
  现在开始搭建属于你的博客.
```


## 一、第一步：下载安装Git
> [Git下载地址](https://gitforwindows.org/)


<!-- more -->

### Git安装步骤
![](https://upload-images.jianshu.io/upload_images/1531909-4da9b2db5ad099b5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/519)


![](https://upload-images.jianshu.io/upload_images/1531909-44bddccbb0bc44fb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/483)
>然后一路默认




## 二、第二步：下载安装node.js

### 1、[node.js下载地址](https://nodejs.org/en/)

![](https://upload-images.jianshu.io/upload_images/1531909-acb3ca9d69e0037f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)
>2、安装步骤：一路默认就行（安装路径根据自己需要更改）

## 三、第三步：安装hexo

> 1、利用 npm 命令即可安装。在任意位置点击鼠标右键，选择Git Bash

![](https://upload-images.jianshu.io/upload_images/1531909-ed306496f5c34312.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/237)

>2、输入命令：npm install -g hexo

![](https://upload-images.jianshu.io/upload_images/1531909-0b9d56643f6b27cc.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/648)

> 注意：-g是指全局安装hexo。

## 四、第四步：初始化Hexo
> 1、创建文件夹（我的是在E盘创建的Hexo--根据个人爱好创建博客文件夹）
![](https://upload-images.jianshu.io/upload_images/1531909-b4cfc9da3f2063b9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/650)

> 2、在Hexo文件下，右键运行Git Bash，输入命令：hexo init
>（这里可能时间会长些，要耐心等待）
![](https://upload-images.jianshu.io/upload_images/1531909-f6ae9b7089741c89.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)

> 初始化成功后生成的一些列文件,如下
![](https://upload-images.jianshu.io/upload_images/1531909-d0452912537c03e8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/658)

> 3、在_config.yml,进行基础配置 (在你创建的博客文件夹（hexo）下的_config.yml文件)

![](https://upload-images.jianshu.io/upload_images/1531909-cd5743eda172deca.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/663)

> 其中可以在这里[浏览更多主题](https://hexo.io/themes/)，然后在Hexo文件夹下 Git Bash(在hexo文件夹下鼠标右键就可以看到GitBash，点击打开)

> 输入命令：git clone https://github.com/iissnan/hexo-theme-next themes/next（next为主题名字），来获得更多主题(我现在在用的主题[shana](https://github.com/ShanaMaid/hexo-theme-shana))

![](https://upload-images.jianshu.io/upload_images/1531909-c428c38d5b6f608d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/537)

![](https://upload-images.jianshu.io/upload_images/1531909-9e10141923fcdf7a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/489)


> 4、本地浏览博客
>  分别输入 如下命令：
>      hexo g
>      hexo s

>  [hexo常用命令](https://segmentfault.com/a/1190000002632530)

![](https://upload-images.jianshu.io/upload_images/1531909-0501276ece21c570.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/566)

#####   在浏览器输入：localhost：4000 ，就可以进行访问，效果如下：
![](https://upload-images.jianshu.io/upload_images/1531909-4f9a111a4f87ff63.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)

#### 5、写文章
> 在E:\Hexo\source\_posts文件下，新建.md文件就可以写文章
![](https://upload-images.jianshu.io/upload_images/1531909-f369abde30af73e0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/478)


> ---
> title: 我的博客
> ---

![](https://upload-images.jianshu.io/upload_images/1531909-a55880ce3bb59600.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/307)
![](https://upload-images.jianshu.io/upload_images/1531909-3b9c7f217892c046.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)


## 五、部署到Github上

> 1、申请Github账号，（注意别忘了进行账号邮箱验证）
> 2.new repository

![](https://upload-images.jianshu.io/upload_images/1531909-8decffce7d3866b3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/494)

![](https://upload-images.jianshu.io/upload_images/1531909-d3da80e668341305.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/469)

> 记得名字要一致。否则部署上GitHub的博客无法正常显示


> 然后点击
![](https://upload-images.jianshu.io/upload_images/1531909-fe29bad673d85f37.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/246)


> 3、在_config.yml进行配置 (注意要保存, 记得要有空格否则报错)
![](https://upload-images.jianshu.io/upload_images/1531909-d0fc558c749b5569.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)


>  4、安装[hexo-deployer-git](https://github.com/hexojs/hexo-deployer-git)自动部署发布工具

>    npm install hexo-deployer-git  --save

![](https://upload-images.jianshu.io/upload_images/1531909-fb7e657ad2729c88.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/354)

> 5、发布到Github
>     输入如下命令：hexo clean && hexo g && hexo d

 ![](https://upload-images.jianshu.io/upload_images/1531909-72b3c30ffbfb1210.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/274)
 ![](https://upload-images.jianshu.io/upload_images/1531909-5fdbcdab2249c01e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/506)

 > 第一次发布需要验证github账号 (部署时可能还会提示你全局绑定github用户名和邮箱)
 ![](https://upload-images.jianshu.io/upload_images/1531909-1f99441c5f2e0cfb.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/359)


 > 发布成功后，我们在仓库中看到这个
 ![](https://upload-images.jianshu.io/upload_images/1531909-eeae3f8de4041eff.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)


 > 6、测试访问
 > 在浏览器输入：https://tuspring.github.io/ (你的repository)

 ![](https://upload-images.jianshu.io/upload_images/1531909-a771d32449cbd5c8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)


 ```angular2html
   最后，搭建完毕！ 噢耶
```