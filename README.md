# Git 学习报告（myl）

## 1. Git 常用指令学习

这次练习主要把最常用的一些命令过了一遍，下面是我自己的理解。

### `git clone`

作用：把远程仓库复制到本地。

```bash
git clone <仓库地址>
```

一般是学习一个项目的第一步，先 clone 下来再改代码。

### `git branch`

作用：查看或创建分支。

```bash
git branch
git branch <新分支名>
```

我理解分支就是“并行开发线”，不影响主分支时就先开新分支。

### `git checkout`

作用：切换分支。

```bash
git checkout <分支名>
```

！！！切分支前最好先确认当前修改是否已经提交，避免切换时混乱。

### `git add`

作用：把工作区修改放到暂存区。

```bash
git add <文件名>  #单个文件
git add .  #所有文件
```

### `git push`

作用：把本地提交推送到远程仓库。

```bash
git push origin <分支名>
```

### `git pull`

作用：拉取远程最新内容并合并到本地。

```bash
git pull origin <分支名>
```

多人协作时这个命令很常用，先 pull 再开发能减少冲突。

---

## 2. Git 提交的命令行输出

```text
myl@LAPTOP-COE4IRUE MINGW64 ~/Desktop/learn_git (myl-my-solution)
$ git push origin myl-my-solution
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 32 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.13 KiB | 1.13 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'myl-my-solution' on GitHub by visiting:
remote:      https://github.com/happywosabi/learn_git/pull/new/myl-my-solution
remote:
To https://github.com/happywosabi/learn_git.git
 * [new branch]      myl-my-solution -> myl-my-solution
```

