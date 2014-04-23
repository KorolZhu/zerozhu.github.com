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

