# git-学习报告
## 一、常用指令学习
|指令|作用|
|---|---|
|git clone|从git服务器拉取代码|
|git config|配置开发者用户名和邮箱|
|git branch|创建、重命名、查看、删除项目分支|
|git checkout|切换分支|
|git status|查看文件变动状态|
|git add|添加文件变动到暂存区|
|git commit|提交文件变动到版本库|
|git push|将本地的代码改动推送到服务器|
|git pull|将服务器上的最新代码拉取到本地|
|git log|查看版本提交记录|
|git tag|为项目标记里程碑|
## 二、git提交命令行输出
```
guichen@guichen-Lenovo-Legion-Y7000P2021:~/Documents/ws/learn_git$ git push origin zbw-my-solution
枚举对象中: 6, 完成.
对象计数中: 100% (6/6), 完成.
使用 16 个线程进行压缩
压缩对象中: 100% (4/4), 完成.
写入对象中: 100% (4/4), 872 字节 | 872.00 KiB/s, 完成.
总共 4（差异 0），复用 0（差异 0），包复用 0
remote: 
remote: Create a pull request for 'zbw-my-solution' on GitHub by visiting:
remote:      https://github.com/happywosabi/learn_git/pull/new/zbw-my-solution
remote: 
To https://github.com/happywosabi/learn_git.git
 * [new branch]      zbw-my-solution -> zbw-my-solution
```