---
layout: page
title: 第三章 Editorial 结构
chapter_title: 第三章 Editorial 结构
permalink: /docs/editorial/
---

Editorial 是一套我们根据 Jekyll 定制的主题，所以这里我们说的 Editorial 的结构是指除了 Jekyll 软件本身的结构之外的我们编辑中可能用到的编辑结构。

## 一 书名和作者

书名和作者我们是在软件的根目录下的 `_config.yml` 中进行定制。

~~~ yaml
# 书名
title: Write book with Editorial
# 作者
author: Huang Feilong
~~~

这两个信息将会在网站页面的右栏上方显示，同时这两个项目生成一个指向网站首页的链接，也是全站唯一一个返回首页的链接。

## 二 联系方式

在页面左侧栏目录下方有一个“联系我”的栏目，那里就是显示作者联系方式的地方。
联系方式的设置同样在 `_config.yml` 中的作者位置下方：

~~~yml
  email: information@untitled.tld
  telephone: (000) 000-0000
  address: 1234 Somewhere Road #8254 Nashville, TN 00000-0000
~~~

## 三 目录

目录目前支持两级目录，也就是章和节。

## 四 著作特色

概述本书的特点，因为排版原因，最好是四大特点。

## 五 编纂日志

为您的日夜的奋斗留下看法、想法和感悟。

## 六 书内搜索

目前该功能还在建设中……

位置已经预留在左侧栏的顶端，但是由于汉字检索的一些问题，目前还需要进一步完善。
