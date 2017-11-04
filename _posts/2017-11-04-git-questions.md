---
layout: post
title: 使用Git遇到的问题
subtitle: subtitle
author: luhggit
date: 2017-11-04 08:30
categories: jekyll
tag: 技术 Linux
---

# [使用Git遇到的问题及解决方法]()

### 已经将SSH公钥生成，将上传到github，但是提交的时候仍然是Permission denied

猜想：ssh公钥是生成到了root用户的文件夹下面，因为当前repository的所有者是root,所以只有root用户才能获取到公钥和私钥

解决方法：将repository的所有者改为当前用户，相当于把当前文件夹的所有权限都赋给了当前用户，但是只要有当前文件夹的权限就可以读取到公钥和私钥吗，还有SSH的传输过程是怎样的？有待解决
