---
layout: post
title: Linux常用操作命令
subtitle: subtitle
author: luhggit
date: 2017-11-04 07:31:27 +0800
categories: jekyll
tag: 技术 Linux
---

# [Linux 常用操作命令]()

## [文件操作相关]()

#### 创建文件
```
sudo touch 文件名
```
#### 创建目录
```
sudo mkdir 目录名
```
#### 移动文件
```
sudo mv 文件名或目录 地址
```

#### 删除文件
```
sudo rm -rf 文件名
```

## [权限操作相关]()
#### 查看当前用户信息
```
cat /opt/passwd
cat /opt/passwd|grep "keyword"
```

注：`grep`关键字是用来对命令的结果进行模糊搜索的？

执行结果如下：
```
luhg:x:1000:1000:luhg,,,:/home/luhg:/usr/bin/zsh

用户名：密码：用户id：用户组id：备注：用户home目录：shell地址

```
注：可以根据用户组id来找到当前用户所在的组

#### 查看当前组信息
```
cat /opt/group
cat /opt/group|grep "keyword"
```
执行结果如下：
```
adm:x:4:syslog,luhg

组名：密码：组id：组成员
```

#### 修改文件夹的所有者（所有者拥有所有的权限）
如：将/opt/luhg-blog文件夹的所有者修改为luhg
```
chown -R luhg /opt/luhg-blog/
```
