---
layout: post
title: "git常用命令"
date: 2014-04-22 22:53:42 +0800
comments: true

---

###1、添加本地项目到GitHub
```
$ cd my_project
$ git init
$ git add *
$ git commit -m "First commit"
$ git remote add origin https://github.com/yourname/my_project.git
$ git pull origin master
$ git push -u origin master

```
###2、分支的删除
   * 删除本地分支

```
$ git branch -d <branchname> （删除已经合并的分支） 
$ git branch -D <branchname> （删除即使没有合并的分支）

```
   * 删除远程分支

```
$ git push origin --delete <branchname>
$ git push origin :<branchname>  (git push [远程名] [本地分支]:[远程分支])

```
###3、获取远程分支
通过git clone获取的远端git库，只包含了远端git库的当前工作分支。如果想获取其它分支信息，需要使用”git branch  –r” 来查看，如果需要将远程的其它分支代码也获取过来，可以使用命令” git checkout -b 本地分支名 远程分支名”，其中，远程分支名为git branch –r所列出的分支名， 一般是诸如“origin/分支名”的样子。如果本地分支名已经存在， 则不需要“-b”参数

```
$ git checkout -b 本地分支名 远程分支名

```


