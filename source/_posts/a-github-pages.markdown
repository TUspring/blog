---
layout: post
title: "GitHub Pages绑定域名"
date: 2016-12-21 18:40
comments: true
tags: 
	- 域名
	- hexo
---

如果你用hexo-github搭了博客，又不想使用GitHub的xxx.github.io,  可以看下面怎么去绑定自己的域名。
（没有域名？[点传送门](https://wanwang.aliyun.com/?spm=5176.8142029.388261.550.a723381fLPFyjm))
###### 1. 向你的 Github Pages 仓库添加一个CNAME(一定要大写)文件
其中只能包含一个顶级域名，像这样：
example.com  ---->注意前面没有http://，也没有www，

还有你用 hexo 框架搭建博客并部署到 Github Pages 上，每次
> hexo g
> hexo d

后会把你的博客所在目录下 public 文件夹里的东西都推到 Github Pages 仓库上，并且把 CNAME 文件覆盖掉，解决这个问题可以直接把 CNAME 文件添加到 source 文件夹里，这样每次推的时候就不用担心仓库里的 CNAME 文件被覆盖掉了。

###### 2. 向你的 DNS 配置中添加 3 条记录
@          A             192.30.252.153
@          A             192.30.252.154
www      CNAME           username.github.io.

用你自己的 Github 用户名替换 username
（其实www的方式，会先解析成http://xxxx.github.io，然后根据CNAME再变成http://xxx.com，即中间是经过一次转换的）。
配置 DNS 推荐使用 DNSPOD 的服务，使用国外的 DNS 解析服务可能有被墙的风险。

