## hyp的git学习报告
### 一.指令学习（部分）
git clone 把远程仓库下载到本地
git add 把文件的改动放入暂存区
git commit -m 把暂存区的改动永久记录到本地仓库历史中
git push origin 把本地提交的改动上传到 GitHub 远程仓库对应分支。
git pull origin 把远程仓库的最新改动拉取到本地，并自动合并到当前分支。
git branch查看本地所有分支，当前所在分支前有 * 标记。加 -a 可查看远程分支。
git checkout 切换到指定分支。
git checkout -b 创建并切换到新分支
### 二.命令行输出
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
