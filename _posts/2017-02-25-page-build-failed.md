---
title: "搭建博客踩坑:page build failed"
date: 2018-02-25 22:30 +0800
categories:
  - tech
tags:
  - 博客
  - bugs
  - github
---
>使用github pages + jekyll搭建的博客

### 问题：push之后生成页面失败 page build failed

- 错误提示：
>"The site configured at this address does not contain the requested file.
If this is your site, make sure that the filename case matches the URL.
For root URLs (like http://example.com/) you must provide an index.html file."

- 经过：2018-02-24 晚上十一点左右开始push没有新页面生成，多次未果；次日晚上继续找原因。清空仓库，重来，更换分支，使用旧代码，又重新使用新主题。再一个个文件复制修改。最终发现是travel.md 文件中语法错误。
- 损失：3个小时浪费在查找原因，重新clone和push上
- 原因：新增的一个页面内容有误，程序不能生成。因为同期push多个页面，导致没有及时发现问题页面为何。
