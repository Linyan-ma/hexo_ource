---
title: GitCommands
date: 2017-12-18 09:29:55
tags:
categories: CODE
---
## git的命令
* git init
* git config --global user.name "Your Name"
* git config --global user.email "email@example.com"
* git remote add origin https://github.com/Linyan-ma/react-Learn.git 连接远程仓库
* git add . (git add --A/git add <file>)
* git commit -m "describe"
* rm -rf .git 删除.git文件
* git config --global core.autocrlf false crlf windows下的空格换行（warning: LF will be replaced by CRLF）
* git rm README.1.md 删除文件
* git push --force origin master 强制push
* git push origin master 提交的远程仓库
* git pull origin master 远程仓库拉取
* git reset --hard HEAD^ （git reset --hard commit_id）回退到上个版本。上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100。
* 
* 其他命令 git status / git log 

git config --global credential.helper store存储用户名密码