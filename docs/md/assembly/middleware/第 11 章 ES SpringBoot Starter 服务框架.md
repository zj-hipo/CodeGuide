---
title: 第 11 章 ES SpringBoot Starter 服务框架
pay: https://t.zsxq.com/0c7qkNTdA
---

# 第 11 章 ES SpringBoot Starter 服务框架

作者：小傅哥
<br/>博客：[https://bugstack.cn](https://bugstack.cn)

>沉淀、分享、成长，让自己和他人都能有所收获！

## 一、前言

`经历过的场景越多，提出解决方案的速度越快`

其实很多时候的很多问题，除了差异也都是具有共性的，经历的场景越多、解决的问题越多，也就会发现这些共性问题的差异并不大，但共性却很相同。

就想我们去开发一个系统、组件、模块，这些各类的实现代码在不同的业务服务中，可能仅仅是一些渠道、参数、类型的差异，而核心代码部分基本都是可以复用的。

这也就是我们常提到的，中间件要解决的是提取业务逻辑中，具有共性通用问题的场景做凝练复用，解决所有同类问题产生。

## 二、需求背景

在数据库 ORM 框架设计中，我们尝试开发一个自己的 ORM SpringBoot Starter 解决系统中对数据库的使用。

同样这里我们也是要解决类似的问题，只不过把数据库换成了 Elasticsearch，把 JDBC 替换为 x-pack-sql-jdbc。有了这些基础组件的提供，就可以开发出一个 ES ORM SpringBoot Starter 的组件，让我们可以轻松的在系统中像使用 MyBatis 一样操作 Elasticsearch 服务。

其实本章节的开发并不复杂，因为我们已经了开发此类 ORM 框架的基础，所以本章节更多的是对 ORM 框架技术的横向复用。