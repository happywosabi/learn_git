# Git

## 1. 常用命令

```bash
git remote add origin <example.git>
```

将当前本地仓库与远程仓库关联。`origin` 是远程仓库的默认别名，后续可以使用它来推送和拉取代码。

### 复制仓库

```bash
git clone <example.git>
```

在当前目录复制远程仓库到本地。

### 分支

```bash
git branch solution/0.0.0
```

创建一个名为 `solution/0.0.0` 的分支。

```bash
git branch -m solution/0.0.0 solution/0.0.1
```

将分支 `solution/0.0.0` 重命名为 `solution/0.0.1`。

```bash
git branch -d solution/0.0.1
```

删除 `solution/0.0.1` 分支。

```bash
git branch
```

查看当前项目所有分支。

### 切换分支

```bash
git checkout solution/0.0.0
```

切换到 `solution/0.0.0` 分支。

```bash
git checkout -b solution/0.0.0
```

创建并切换到 `solution/0.0.0` 分支。

### 添加文件

```bash
git add README.md
```

将文件 `README.md` 添加到暂存区。

```bash
git add .
```

将所有文件添加到暂存区。

### 推送

```bash
git push origin solution/0.0.1
```

将 `solution/0.0.1` 分支推送到服务器。

### 拉取

```bash
git pull origin solution/0.0.1
```

将远程仓库 `solution/0.0.1` 分支改动更新到本地。

---
