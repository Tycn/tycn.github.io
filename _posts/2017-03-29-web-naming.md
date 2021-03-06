---
layout: post
title:  "前端开发中常用命名规则"
categories:  前端开发
tags:  HTML CSS JavaScript
author: Tycn
---

* content
{:toc}
## HTML命名规范

### 文件名

| 内容                 | 文件命名               | 例子               |
| ------------------ | ------------------ | ---------------- |
| List Page          | fileName + s       | users.html       |
| Detail Page        | fileName + Info    | userInfo.html    |
| Data / Update Page | fileName + Act     | userAct.html     |
| Update Page        | fileName + Edit    | userEdit.html    |
| Insert Page        | fileName + Add     | userAdd.html     |
| Delete Page        | fileName + Delete  | userDelete.html  |
| Order Page         | fileName + Order   | userOrder.html   |
| Data Validate Page | fileName + Checker | userChecker.html |



- default/index.html    首页
- 404.html              404错误页
- print.html            打印页
- header.html           页头
- footer.html           页脚
- sitemap.html          网站地图
- passport.html         通行证
- rank.html             排行榜
- roll.html             滚动新闻
- solution.html         解决方案
- joinus.html           加入我们
- partner.html          合作伙伴
- service.html          服务
- aboutus.html          关于我们
- contact.html          联系我们
- company.html          公司介绍
- organization.html     组织结构
- culture.html          企业文化
- strategy.html         发展策略
- honor.html            公司荣誉
- aptitudes.html        企业资质
- events.html           大事记
- business.html         商务合作
- contract.html         服务条款
- privacy.html          隐私声明
- CSR.html              企业社会责任
- news-开头.html         新闻相关
- article-开头.html      资讯相关
- picture-开头.html      图片相关
- photo-开头.html        相册相关
- product-开头.html      产品相关
- goods-开头.html        商品相关
- system-开头.html       系统相关
- tag-开头.html          tag相关
- brand-开头.html        品牌相关
- help-开头.html         帮助相关
- member-开头.html       会员相关
- search-开头.html       搜索相关

## CSS命名规范

### 类名

| 内容                              | 类(文件)名            | 例子             |
| ------------------------------- | ----------------- | -------------- |
| Interface                       | I + ClassName     | IParamLanguage |
| Model                           | ClassName + Model | UserModel      |
| DAL 数据访问层(Data Access Layer)    | ClassName + DAL   | ……             |
| BLL 业务逻辑层(Business Logic Layer) | ClassName + BLL   | ……             |

### 主体

- 头部：header
- 内容：content/container
- 尾部：footer
- 导航：nav
- 侧栏：sidebar
- 栏目：column
- 整体布局：wrapper
- 左右中：left / right / center
- 登录条：loginbar
- 标志：logo
- 广告：banner
- 页面主体：main
- 热点：hot
- 新闻：news
- 下载：download
- 子导航：subnav
- 菜单：menu
- 子菜单：submenu
- 搜索：search
- 友情链接：friendlink
- 页脚：footer
- 版权：copyright
- 滚动：scroll
- 标签页：tab
- 文章列表：list
- 提示信息：msg
- 小技巧：tips
- 栏目标题：title
- 加入：join
- 指南：guild
- 服务：service
- 注册：regsiter
- 状态：status
- 投票：vote
- 合作伙伴：partner

### id的命名规范

#### 1. 页面结构

- 容器: container
- 页头：header
- 内容：content/container
- 页面主体：main
- 页尾：footer
- 导航：nav
- 侧栏：sidebar
- 栏目：column
- 页面外围控制整体布局宽度：wrapper
- 左右中：left right center

#### 2. 导航

- 导航：nav
- 主导航：mainnav
- 子导航：subnav
- 顶导航：topnav
- 边导航：sidebar
- 左导航：leftsidebar
- 右导航：rightsidebar
- 菜单：menu
- 子菜单：submenu
- 标题：title
- 摘要：summary

#### 3. 功能

- 标志：logo
- 广告：banner
- 登陆：login
- 登录条：loginbar
- 注册：regsiter
- 搜索：search
- 功能区：shop
- 标题：title
- 加入：joinus
- 状态：status
- 按钮：btn
- 滚动：scroll
- 标签页：tab
- 文章列表：list
- 提示信息：msg
- 当前的：current
- 小技巧：tips
- 图标：icon
- 注释：note
- 指南：guild
- 服务：service
- 热点：hot
- 新闻：news
- 下载：download
- 投票：vote
- 合作伙伴：partner
- 友情链接：link
- 版权：copyright

#### 4. class的命名

- 颜色：使用颜色的名称或者16进制代码，如：

  > .red { color: red; } .f60 { color: #f60; } .ff8600 { color: #ff8600; }

- 字体大小，直接使用“font+字体大小”作为名称，如：

  > .font12 { font-size: 12px; }

- 对齐样式，使用对齐目标的英文名称，如：

  > .flt {float: left} .frt { float: right}

- 标题栏样式，使用“类别+功能”的方式命名，如：

  > .bar-news { } .bar-product { }

### 样式文件命名

- 主要的:master.css
- 布局版面:layout.css
- 专栏:columns.css
- 文字:font.css
- 打印样式:print.css
- 主题:themes.css

### 声明顺序

CSS 声明顺序以类型（position, display, colors, font, miscellaneous…）顺序排列，依赖盒模型定义顺序：由外而内。

> 1.位置属性(position, top, right, z-index, display, float等)
> 2.大小(width, height, padding, margin)
> 3.文字系列(font, line-height, letter-spacing, color- text-align等)
> 4.背景(background, border等)
> 5.其他(animation, transition等)

```
.class {
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  width: 100px;
  height: 100px;
  padding: 0;
  margin: 0;
  font-size: 1.5em;
  font-weight: bold;
  line-height:30px;
  color: #fff;
  background: #08c;
  overflow: hidden;
}
```

### 注意事项

1. 一律小写；
2. 尽量用英文；
3. 尽量不加中杠和下划线；
4. 尽量不缩写，除非一看就明白的单词，如：wrapper可以写成wrap。
5. css文件命名规范：
   - 主要的 master.css
   - 模块 module.css
   - 基本共用 base.css
   - 布局，版面 layout.css
   - 主题 themes.css
   - 专栏 columns.css
   - 文字 font.css
   - 表单 forms.css
   - 补丁 mend.css
   - 打印 print.css

## JavaScript

### JavaScript 注释规范

```
/*
 * 文档注释写在这里
 * @alias aliasName (使用@alias可以给一个变量或者函数指定一个别名，代码提示时会提示该别名)
 * @description 描述内容 ([email protected]�者函数的描述信息。)
 * @example 示例内容 (使用@example可以提示代码示例。)
 * @extends {Type} (使用@extends用于标识继承于某个类型。)
 * @param {Type[,Type,...]} ParameterName=[Value1|Value2[|Value3|...]] 参数描述 (使用@param可以描述一个函数的参数以及参数类型，HBuilder扩展了参数值域的写法（目前只支持字符串值域）)
 * @property {Type[,Type,...]} propertyName 属性描述 (使用@property可以描述一个对象的属性)
 * @constructor (使用@constructor可以标识一个函数是构造函数)
 * @type {Type[,Type,...]} (使用@type可以定义某个变量的类型)
 * @return {Type[,Type,...]} (使用@return可以描述一个对象的属性)
 * @throw {TypeError} 参数类型不匹配 (异常信息)
 */
 function add(item){
    if(typeof item === "number"){
        arr.push(item)
    }
    else{
        throw new TypeError();
    }
}
```

