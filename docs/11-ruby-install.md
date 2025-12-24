---
layout: page
title: 第一节 Ruby 的安装与使用
chapter_title: 第一章 系统构建
permalink: /docs/ruby/
---

## Ruby 语言

### 为什么是 Ruby？

因为我们选择的数字文献发布平台的底层就是使用 Ruby 语言构建，所以我们要先介绍一下 Ruby。

### Ruby 是什么？

Ruby 是红宝石！当然了，英文 Ruby 的中文意思就是红宝石。但是，我们这里的 Ruby 指的是一种编程语言——一种号称“程序员最好的朋友”的编程语言。

Ruby 语言使用起来简洁、易懂，个人认为更适合我们国人使用。虽然总是因为“运行速度”遭人诟病，但是对于你我对于速度不敏感的人来说，无伤大雅。实际上，这个速度问题感觉就像20年前人们诟病的软件大小问题一样，随着数码设备的逐渐升级，这并不是问题。

Ruby 的软件通常会打包成一个个 Gem 的形式来发行，就像 Windows 上的可执行文件 `.exe` 形式，或者我们平时传送文件时会将文件压缩为一个个压缩包一样。

### 安装 Ruby

Ruby 语言是开源免费的自由软件，每个人可以无偿免费随意使用。使用前，当然需要在您的本地计算机上安装了。安装 Ruby，可以根据您使用的操作系统不同，可以安装方法不同。

#### Windowns 下安装 Ruby

在 Windows 系统下，安装 Ruby，有个不错的项目能帮你安装 Ruby：[RubyInstaller](http://railsinstaller.org/)。它能帮你在 Windows 中安装所需的所有 Ruby 开发环境。

#### 其他平台

可以使用多种工具安装 Ruby。本页介绍如何使用主流的包管理系统和第三方工具管理和安装 Ruby，以及如何通过源码编译安装。参考https://www.ruby-lang.org/zh_cn/documentation/installation/

## Gem 和 Bundle

Ruby 从诞生起就开始使用 Gem 软件管理系统来管理 Ruby 软件，而 Bundler 就是基于 Gem 开发的一个大管家。

### Gem

Ruby 软件通常都会打包成 Gem 形式进行发布和安装，Gem 软件的一个集中托管网站就是 [Ruby Gems](https://rubygems.org)。

Gem 软件的安装：

~~~ruby
gem install rails
~~~

Gem 软件的卸载：

~~~ruby
gem uninstall rails
~~~

所以，如果需要安装 Jekyll 软件，则

~~~ruby
gem install jekyll
~~~

### Bundler

通常一个系统可能会用到很多的 Gem 软件，这些软件之间会有互相依赖的关系。单靠 Gem 自身是很难管理的，于时 [Bundler](https://bundler.io) 应运而生。

Bundler 会检查软件的依存关系，然后根据关系进行批量安装。

Bundler 的命令是 `bundle`。

上面我们已经安装完 Jekyll，接下来就可以使用 Jekyll 软件的命令建立网站了。

~~~bash
jekyll new book-site
~~~

上面建立的站点名字就是 `book-site`，然后我们就进入该目录，检查软件依赖是否健全。

~~~ bash
cd book-site
bundle
~~~

这样我们就会看到 Bundler 在检查依赖软件，如果有缺失就会安装。安装结束就可以使用 Jekyll 软件了。

很多时候，可能我们安装的软件与本地软件会有冲突，例如我们安装的 Jekyll 是 3.5 版本，但是本地的 Jekyll 的版本是 3.6。那么就有版本冲突的问题，要升级安装的 Jekyll 到 3.6 才能运行，要么需要使用 Bundler 启动版本保护，通过 `bundle exec jekyll server` 来使用原来的 3.5 版本。
