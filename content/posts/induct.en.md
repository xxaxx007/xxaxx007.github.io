---
title: "Induct"
subtitle: ""
author: ""
date: 2022-12-20T20:57:03+08:00
lastmod: 2022-12-20T20:57:03+08:00
draft: false
description: ""
images: []
password: 123xxaxx321
tags: []
categories: []

twemoji: false
---



### 常用工具指令一览表

#### `git`

* git init
* git config
* git clone
* git add
* git comment -m ""
* git pull
* git push
* git remote -v
* git branch
* git checkout
* git set --soft

#### `vim`

* 上下左右后移动：`kjhlb` ,同时可以用数字快速移动：`3j` 表示向下移动三行
* 插入：`o` 表示下一行，`i` 和 `I` 表示光标后以及行首，而 `a` 恰恰相反：`a` 表示光标后, `A` 表示行尾
* 全选复制：`yie`
* 全部删除：`ggdG`
* 从当前复制到结尾：`yG`
* 从当前到结尾复制：`y$`
* 分别快速跳转到行首、尾快捷键：`H`、`L`

#### `docker`

* docker images：查看镜像
* docker pull
* docker ps -a ：查看进程
* docker stop
* docker rmi :删除镜像
* docker rm $(docker ps -a -q)：删除容器

#### 搭建 `markdown` 图床

* 测试结果如下：
 ![avatar](https://cdn.jsdelivr.net/gh/xxaxx007/mkImg/images/avatar.png) 
  
* 自定义名字
  ![custom-name](https://cdn.jsdelivr.net/gh/xxaxx007/mkImg/images/custom-name.png)

* 快捷键使用
  `ctrl + Alt + u` 、`ctrl + Alt + e` 和 `ctrl + Alt + o`
![test](https://raw.githubusercontent.com/xxaxx007/mkImg/main/images/test.jpg)
* 启用 CDN 加速
 ![1227](https://cdn.jsdelivr.net/gh/xxaxx007/mkImg@main/images/1227.png)
