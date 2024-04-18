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
> - 了解RuoYi-Cloud项目结构
> - 熟悉Docker虚拟容器
> - 熟悉Docker-Compose编排工具


#### ⒈Clone RuoYi-Cloud代码到本地。

+ 使用git clone命令从托管平台Gitee克隆【**[RuoYi-Cloud](https://gitee.com/y_project/RuoYi-Cloud)**】代码。

#### ⒉修改微服务中Nacos的服务注册地址和配置中心地址。

+ 修改ruoyi-auth、ruoyi-gateway、ruoyi-file、ruoyi-gen、ruoyi-job、ruoyi-system和ruoyi-visual服务中配置文件bootstrap.yml（src\main\resources目录）中配置的注册中心和配置中心默认地址，
+ 将127.0.0.1:8848修改为ruoyi-nacos:8848

#### ⒊打包服务端各个服务为jar

+ 打开RuoYi-Cloud\bin目录，双击运行package.bat，将各个微服务进行打包。
+ 将各个服务打包后的jar拷贝到RuoYi-Cloud\docker\ruoyi对应的各个目录中。（比如：RuoYi-Cloud\ruoyi-auth\target\ruoyi-auth.jar拷贝到RuoYi-Cloud\docker\ruoyi\auth目录，以此类推）


#### ⒋编译前端项目为静态文件

+ 打开RuoYi-Cloud\ruoyi-ui\bin目录，双击运行build.bat，编译前端项目。
+ 将编译好的RuoYi-Cloud\ruoyi-ui\dist目录整体拷贝到RuoYi-Cloud\docker\nginx\html目录。

#### ⒌放置数据库脚本到Docker目录

+ 将RuoYi-Cloud\sql目录下所有*.sql文件拷贝到RuoYi-Cloud\docker\mysql\db目录。

#### ⒍将整个RuoYi-Cloud\docker上传到服务器

+ 将RuoYi-Cloud\docker整体上传到服务器/home/ruoyi目录(可以自行定义)。
+ cd到服务器/home/ruoyi/docker目录，执行chmod +x deploy.sh命令，给deploy.sh脚本赋予执行权限。

#### ⒎构建项目中定义的服务容器

+ 使用docker-compose build命令构建服务容器。

#### ⒏启动服务

+ 执行./deploy.sh base命令启动基础服务。
+ 登录nacos服务，修改各个服务配置中的redis和mysql连接地址为docker-compose.yml定义的相应的服务名称。
+ 执行./deploy.sh modules命令启动程序模块。

同步视频教程：
<iframe width="560" height="315" src="https://www.youtube.com/embed/G0WtfMyRI_M?si=mimmqujTy2KQVXWG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>ss