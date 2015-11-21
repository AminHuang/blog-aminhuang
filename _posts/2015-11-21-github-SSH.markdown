---
layout: post
title:  "github SSH"
date:   2015-11-21 20:12:00
---

# 配置SSH keys

## 检查 SSH kyes 的设置

首先检查电脑上的ssh key：

```
$ cd ~/.ssh 检查本机ssh密钥
```

## 生成新的SSH keys

```
$ ssh-keygen -t rsa -C "邮件地址@youremail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/your_user_directory/.ssh/id_rsa):<回车就好>
```
