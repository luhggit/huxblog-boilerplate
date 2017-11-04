---
layout: post
title: Git常用操作命令
subtitle: subtitle
author: luhggit
date: 2017-11-04 07:31:27 +0800
categories: jekyll
tag: 技术 Linux
---

# [Git常用操作命令]()

```
git diff
```
查看未加入暂存区的文件的具体修改，即git add 之前所做的修改

```
git diff --cached
```
查看加入了暂存区的文件的修改，即git add 之后所做的修改

```
git status
```
查看暂存区的状态，即哪些文件做了修改，哪些文件修改了没有add,哪些文件是新添加的（未被跟踪）

```
git remote -v
```
查看**当前repository**下远程主机的信息，**不同的的repository有不同的remote**
