---
title: "使用 docker 管理 mysql 的基本指令"
subtitle: ""
author: ""
date: 2022-12-30T11:28:49+08:00
lastmod: 2022-12-30T11:28:49+08:00
draft: false
description: "学习使用数据库相关指令"
images: []

tags: []
categories: []

twemoji: true
---
### 使用 docker 管理 mysql

#### 常用指令

* 拉取镜像 `docker pull mysql:latest`
* 查看镜像 `docker images` 和进程 `docker ps -a`
* 暂停和删除进程 `docker stop $(docker ps -aq)` 和 `docker rm $(docker ps -a -q)`
* 启动镜像 `docker run -itd --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql`
* 采用 `bash` 进入 `mysql` : `docker exec -it mysql bash`
* 登录 mysql ：`mysql -u root -p`
* 显示所有数据库：`SHOW DATABASES;`
* 切换数据库：`use databasesname;`
* 设置远程访问权限：`ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY 'mysqlroot';` 和 `grant all privileges on *.* to 'xxaxx'@'%' with grant option;`
* 查看 `ip` ，选择 `navicat` 成功实现远程连接访问：
  
  本地：
  ![1672411623136](image/1672411623136.png)

  `assets/images`:
  ![1672410747865](images/1672410747865.png)

  采用 cdn 加速之后的截图如下：

  ![1672409683896](https://cdn.jsdelivr.net/gh/xxaxx007/mkImg/images/1672409683896.png)

#### 工作小结

经过以上步骤，成功利用 docker 实现从部署、配置到应用的实现，与此同时，掌握了相关工具的基本使用指令。
