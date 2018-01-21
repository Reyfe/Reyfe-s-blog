---
layout: post
title:  "我的第一篇Github博客"
categories: Other
tags:  Other
author: Yubo
---

* content
{:toc}

迟来的一篇博客，作为一个计算机/软件工程的学生居然现在开始用Github写博客，不知道自己以前真是干什么去了，不过现在也还来的及。这就是我的第一篇博客，先用来熟悉Markdown的语法也不错。




## 介绍Markdown

Markdown 是一种用来写作的轻量级「标记语言」，它用简洁的语法代替排版。
读研时写论文使用的是Latex，感觉markdown和latex的思想有些像，都是使用标记来进行组织结构，不过Latex我也至今没有搞清楚很多东西，都是使用的模板，惭愧。

优点
- 专注你的文字内容而不是排版样式，安心写作。
- 轻松的导出 HTML、PDF 和本身的 .md 文件。
- 纯文本内容，兼容所有的文本编辑器与字处理软件。
- 随时修改你的文章版本，不必像字处理软件生成若干文件版本导致混乱。
- 可读、直观、学习成本低。

## 基本语法

### 标题

标题是每篇文章都需要也是最常用的格式，在 Markdown 中，如果一段文字被定义为标题，只要在这段文字前加 \# 号即可。

\# 一级标题

\#\# 二级标题

\#\#\# 三级标题

### 列表

熟悉 HTML 的同学肯定知道有序列表与无序列表的区别，在 Markdown 下，列表的显示只需要在文字前加上 - 或 * 即可变为无序列表，有序列表则直接在文字前加1. 2. 3. 符号要和文字之间加上一个字符的空格

- 列表1
- 列表2
- 列表3

### 引用

如果你需要引用一小段别处的句子，那么就要用引用的格式。

>例如这样

只需要在文本前加入 \> 这种尖括号（大于号）即可

### 图片与链接
插入链接与插入图片的语法很像，区别在一个 !号

图片为：\!\[\]\(\)

链接为：\[\]\(\)

插入图片的地址需要图床，这里推荐围脖图床修复计划 与 CloudApp 的服务，生成URL地址即可。

### 粗体与斜体
Markdown 的粗体和斜体也非常简单，用两个 \* 包含一段文本就是粗体的语法，用一个 \* 包含一段文本就是斜体的语法。

例如：**这里是粗体** *这里是斜体*

### 表格
表格是我觉得 Markdown 比较累人的地方，例子如下：

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

个人PS：比latex的还是要友好一些的。。。

### 代码框
如果你是个程序猿，需要在文章里优雅的引用代码框，在 Markdown下实现也非常简单，只需要用两个 ` 把中间的代码包裹起来。

```js
let getRemainTime = (endTime, deviceTime, serverTime) => {
    let t = endTime - Date.parse(new Date()) - serverTime + deviceTime
    let seconds = Math.floor((t / 1000) % 60)
    let minutes = Math.floor((t / 1000 / 60) % 60)
    let hours = Math.floor((t / (1000 * 60 * 60)) % 24)
    let days = Math.floor(t / (1000 * 60 * 60 * 24))
    return {
        'total': t,
        'days': days,
        'hours': hours,
        'minutes': minutes,
        'seconds': seconds
    }
}
```js


### 分割线
分割线的语法只需要三个 * 号，例如：
***