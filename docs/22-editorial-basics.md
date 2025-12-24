---
layout: page
title: 第二节 Editorial 编辑基础
chapter_title: 第二章 编辑基础
permalink: /docs/editorial-basics/
---

Editorial 是定制的一套 Jekyll 主题，所以很多网页元素会有不一样的页面表现。

## 标题

由于一级标题系统默认已经占用，所以内容标题从二级标题开始，然后依次是三级标题、四级标题，更深层的标题应该用不上了。推荐使用 atx 格式标题：

~~~
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
~~~

## 列表

当内容中包含有列表的时候，可以使用常见的有序列表和无序列表。

### 有序列表

1. 项目一
2. 项目二
3. 项目三

### 无序列表

* 项目A
* 项目B
* 项目C

alt 风格无序列表：

* 项目A
* 项目B
* 项目C
{: .alt}

### 定义列表

术语一
: Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Lorem ipsum dolor.

术语二
: Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Lorem ipsum dolor.

术语三
: Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent. Lorem ipsum dolor.

## 块引用

引用名人名言等可以使用这种方法。

> 时间就像海绵里的水，只要愿意挤，总是还有的。
>
> ——鲁迅

## 表格

### 默认表格

|Name|Description|Price|
|:----:|:-------|:------:|
|Item1|Ante turpis integer aliquet porttitor.|29.99|
|Item2|Vis ac commodo adipiscing arcu aliquet.|19.99|
|Item3|Morbi faucibus arcu accumsan lorem.|29.99|
|Item4|Vitae integer tempus condimentum.|19.99|
|Item5|Ante turpis integer aliquet porttitor.|29.99|
|===============
|||100.00|

### alt 风格表格

|Name|Description|Price|
|:----:|:-------|:------:|
|Item1|Ante turpis integer aliquet porttitor.|29.99|
|Item2|Vis ac commodo adipiscing arcu aliquet.|19.99|
|Item3|Morbi faucibus arcu accumsan lorem.|29.99|
|Item4|Vitae integer tempus condimentum.|19.99|
|Item5|Ante turpis integer aliquet porttitor.|29.99|
|===============
|||100.00|
{: .alt}

## 图像

### 自适应（.fit)

![自适应图像](/assets/images/title.jpg){: .image .fit}

### 靠左还是靠右

![图像靠左](/assets/images/pic.jpg){: .image .left}
Lorem ipsum dolor sit accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.
Lorem ipsum dolor sit accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.

![图像靠右](/assets/images/pic.jpg){: .image .right}
Lorem ipsum dolor sit accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.
Lorem ipsum dolor sit accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.

## 方盒（Box）

Lorem ipsum dolor sit accumsan interdum nisi, quis tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent tincidunt felis sagittis eget. tempus euismod. Vestibulum ante ipsum primis sagittis eget. tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.
{: .box}

## 代码预置块

~~~
i = 0;

while (!deck.isInOrder()) {
    print 'Iteration ' + i;
    deck.shuffle();
    i++;
}

print 'It took ' + i + ' iterations to sort the deck.';
~~~
