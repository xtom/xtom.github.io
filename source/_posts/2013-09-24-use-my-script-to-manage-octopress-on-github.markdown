---
layout: post
title: "Use My Script to Manage Octopress on Github"
date: 2013-09-24 15:39
comments: true
categories: tmp
---

为了在多台电脑之间，编辑放在github上的octopress博客，查阅网络资源后写了cloneblog.sh。 当前提条件都准备好后，运行脚本，我的octopress仓库的master分支和source分支便躺在了当前目录的octopress目录下和octopress/_deploy目录下，它们中分别存放了octopress博客源文件和发布的静态博客页面文件。

为了方便每次写博客前先同步一下github博客仓库，我写了pullblog.sh脚本。它会将github博客仓库上的source分支和master分支更新到本地仓库。

一个不是很实用的脚本，newpost.sh新建博文，此脚本只是简单的封装了一下rake new_post["..."]指令

为了方便每次写完博客，即使更新到github博客仓库，写了pullblog.sh脚本。它将发布本地博文到github博客仓库的master分支，并把博客源代码更新到github仓库的source分支。

目前还只是满足自己用，博客仓库地址都是写死在脚本里的，不可配置。当然感兴趣的伙伴可以参考交流。

下载地址：https://github.com/xtom/kit
