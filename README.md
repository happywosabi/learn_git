# Git 学习报告 - hyp

## 一、常用指令学习

| 指令 | 功能说明 |
|------|----------|
| `git clone <仓库地址>` | 将远程仓库完整下载到本地 |
| `git add <文件>` | 把文件的改动放入暂存区（购物车） |
| `git commit -m "说明"` | 将暂存区的改动永久记录到本地仓库历史 |
| `git push origin <分支名>` | 将本地提交上传到 GitHub 远程仓库的对应分支 |
| `git pull origin <分支名>` | 拉取远程仓库的最新改动并自动合并到当前分支 |
| `git branch` | 查看本地所有分支，当前分支前有 `*` 标记 |
| `git branch -a` | 查看所有分支（包括远程分支） |
| `git checkout <分支名>` | 切换到指定分支 |
| `git checkout -b <新分支名>` | 创建新分支并立即切换到该分支 |

## 二、完成 Git 提交的命令行输出

```bash
$ git push origin hyp-homework
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 32 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 1.10 KiB | 1.10 MiB/s, done.
Total 7 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'hyp-homework' on GitHub by visiting:
remote:      https://github.com/happywosabi/learn_git/pull/new/hyp-homework
remote:
To github.com:happywosabi/learn_git.git
 * [new branch]      hyp-homework -> hyp-homework