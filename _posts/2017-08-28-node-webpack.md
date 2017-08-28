---
layout: post
title:  "初次接触webpack，一边折腾，一边学习！"
categories:  webpack
tags:  webpack npm
author: Tycn





---

* content
{:toc}
**初次接触webpack，一边折腾，一边学习！以下是学习记录：**



1、在node官网下载了node.js v6.11.2  地址：https://nodejs.org/zh-cn/

2、安装好node后在终端检查是否安装正确（显示版本号表示正确）

> ```
> $ node -v
> 显示：v6.11.2
> ```

3、新版node集成了npm，检查一下npm是否安装正确（显示版本号表示正确）

> ```
> $ npm -v
> # 显示：3.10.10
> ```

4、全局安装webpack

> ```
> $ npm install -g webpack
> ```

5、进入项目根目录将 Webpack 安装到项目的依赖中，这样就可以使用项目本地版本的 Webpack

> ```
> # 进入项目目录
> # 确定已经有 package.json，没有就通过 npm init 创建(可以事先拷贝这些文件到目录下，就不需要执行npm init)
> # 安装 webpack 依赖
> $ npm install webpack --save-dev
> ```

6、安装Webpack 开发工具, webpack-dev-server 开发服务，启用localhost:8080

> ```
> $ npm install webpack-dev-server --save-dev
> # 不加-g，在项目根目录出现node_modules文件夹，内含webpack-dev-server及其依赖包
> ```

7、启用server，启用浏览器打开[http://localhost:8080/](http://localhost:8080/)  查看页面

> ```
> $ webpack-dev-server
> # 执行命令后出现报错，Error: Cannot find module 'extract-text-webpack-plugin'
> # 原因分析：npm install webpack-dev-server --save-dev 没有加 -g 全局安装
> # 解决办法：安装extract-text-webpack-plugin
> $ npm install --save extract-text-webpack-plugin
> # 此时在执行 webpack-dev-server 
> $ webpack-dev-server
> # 服务开启，可以在http://localhost:8080/ 查看页面
> ```



后续学习中遇到问题再更新吧……







