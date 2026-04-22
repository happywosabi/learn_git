# Git 学习篇
## 1. git pull origin <分支名> 目前进度：
- [x] 完成addition.cpp
- [ ] 正在进行中🔥🔥🔥
  
常见git command
   | 指令 | 说明 |
   |:---:|:---:|
   |git clone <仓库地址>|将远程仓库完整下载到本地|
   |git add <文件>|把文件的改动放入暂存区（购物车）|
   |git commit -m "说明"|将暂存区的改动永久记录到本地仓库历史|
   |git push origin <分支名>|将本地提交上传到 GitHub 远程仓库的对应分支|
   |git pull origin <分支名>|拉取远程仓库的最新改动并自动合并到当前分支|
   |git checkout daily/0.0.1|切换到 daily/0.0.1 分支，后续的操作将在这个分支上进行|
   |git status|通过 git status 命令可以看到文件当前状态 Changes not staged for commit:（改动文件未提交到暂存区）|

## 2.Git提交的命令行输出:
```
E:\RM_algorithm\learn_git>git push origin wql_my_solution
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 24 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.03 KiB | 1.03 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'wql_my_solution' on GitHub by visiting:
remote:      https://github.com/happywosabi/learn_git/pull/new/wql_my_solution
remote: 
To https://github.com/happywosabi/learn_git.git
 * [new branch]      wql_my_solution -> wql_my_solution
```
