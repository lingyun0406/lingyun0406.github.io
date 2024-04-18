---
layout: post
title: "使用Docker-Compose快速部署开源若依管理系统RuoYi-Cloud版"
date: 2024-04-18 18:45:00
subtitle: "应用容器部署系统"
author: "lingyun0406"
header-style: text
catalog: true
tags:
  - 若依
  - RuoYi-Cloud
  - Docker
  - Docker-Compose
  - Nginx
  - Mysql
  - Redis
---


> 课程前置条件：
>
> - 了解RuoYi-Cloud项目结构
> - 熟悉Docker虚拟容器
> - 熟悉Docker-Compose编排工具


#### ⒈Clone RuoYi-Cloud代码到本地。

+ 使用`git clone`命令从托管平台Gitee克隆【**[RuoYi-Cloud](https://gitee.com/y_project/RuoYi-Cloud)**】代码。

#### ⒉修改微服务中Nacos的服务注册地址和配置中心地址。

+ 修改***ruoyi-auth***、***ruoyi-gateway***、***ruoyi-file***、***ruoyi-gen***、***ruoyi-job***、***ruoyi-system***和***ruoyi-visual***服务中配置文件**bootstrap.yml**（**src\main\resources**目录）中配置的注册中心和配置中心默认地址，
+ 将[127.0.0.1:8848]()修改为[ruoyi-nacos:8848]()

#### ⒊打包服务端各个服务为jar

+ 打开**RuoYi-Cloud\bin**目录，双击运行**package.bat**，将各个微服务进行打包。
+ 将各个服务打包后的**jar**拷贝到**RuoYi-Cloud\docker\ruoyi**对应的各个目录中。（比如：**RuoYi-Cloud\ruoyi-auth\target\ruoyi-auth.jar**拷贝到**RuoYi-Cloud\docker\ruoyi\auth**目录，以此类推）


#### ⒋编译前端项目为静态文件

+ 打开**RuoYi-Cloud\ruoyi-ui\bin**目录，双击运行**build.bat**，编译前端项目。
+ 将编译好的**RuoYi-Cloud\ruoyi-ui\dist**目录整体拷贝到**RuoYi-Cloud\docker\nginx\html**目录。

#### ⒌放置数据库脚本到Docker目录

+ 将**RuoYi-Cloud\sql**目录下所有***.sql**文件拷贝到**RuoYi-Cloud\docker\mysql\db**目录。

#### ⒍将整个RuoYi-Cloud\docker上传到服务器

+ 将**RuoYi-Cloud\docker**整体上传到服务器**/home/ruoyi**目录(可以自行定义)。
+ `cd`到服务器**/home/ruoyi/docker**目录，执行`chmod +x deploy.sh`命令，给**deploy.sh**脚本赋予执行权限。

#### ⒎构建项目中定义的服务容器

+ 使用`docker-compose build`命令构建服务容器。

#### ⒏启动服务

+ 执行`./deploy.sh base`命令启动基础服务。
+ 登录**nacos**服务，修改各个服务配置中的**redis**和**mysql**连接地址为**docker-compose.yml**定义的相应的服务名称。
+ 执行`./deploy.sh modules`命令启动程序模块。
同步视频教程：
<iframe width="560" height="315" src="https://www.youtube.com/embed/G0WtfMyRI_M?si=mimmqujTy2KQVXWG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>ss