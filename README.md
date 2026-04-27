Git 标准使用流程
一、初始环境配置（仅首次使用执行）
1. 安装 Git
官方下载地址：https://git-scm.com/，默认安装即可。
2. 全局账号配置
配置与代码托管平台一致的用户名、邮箱，保证提交记录有效
# 配置全局用户名
git config --global user.name "自定义用户名"

# 配置全局邮箱
git config --global user.email "自定义邮箱"

# 查看配置是否生效
git config --list
二、项目初始化两种场景
场景1：本地已有项目，关联远程仓库
# 进入项目根目录
cd 你的项目本地路径

# 初始化本地git仓库
git init

# 关联远程仓库地址（GitHub/Gitee/GitLab）
git remote add origin 远程仓库HTTPS/SSH地址

# 校验远程关联状态
git remote -v
场景2：拉取远程已有项目到本地
# 克隆远程完整项目
git clone 远程仓库地址
三、标准日常开发流程（核心规范）
核心原则：禁止直接在 main/master 主分支开发，所有功能、Bug 修复均使用独立分支
1. 开发前同步远程最新代码
# 切换到主分支
git checkout main

# 拉取远程最新代码，保证本地代码最新
git pull origin main
2. 创建专属开发分支
# 创建并切换到功能分支
# 规范命名：feature/功能名称、fix/bug问题名称
git checkout -b feature/xxx功能开发
git checkout -b fix/xxxbug修复
3. 代码开发与本地提交
# 查看文件修改状态
git status

# 添加所有修改、新增文件到暂存区
git add .

# 提交代码，填写规范提交备注
git commit -m "feat: 新增xxx功能"
4. 推送本地分支到远程仓库
# 首次推送需要关联远程分支
git push -u origin 分支名

# 后续重复推送直接执行
git push
5. 远程合并代码（PR/MR）
1. 登录代码托管平台，新建 Pull Request / Merge Request
2. 源分支：个人开发分支，目标分支：main 主分支
3. 填写修改说明，提交审核，等待合并
6. 合并后同步清理代码
# 切换回主分支
git checkout main

# 拉取合并后的最新代码
git pull origin main

# 删除本地已合并的无用分支（可选）
git branch -d 分支名

四、高频常用命令大全
# 查看本地所有分支
git branch

# 切换已有分支
git checkout 分支名

# 放弃工作区未提交的修改
git checkout -- 文件名
git checkout -- .

# 查看版本提交日志
git log

# 撤销最近一次commit（保留代码修改）
git reset --soft HEAD^

# 强制拉取远程代码（覆盖本地未提交修改，谨慎使用）
git fetch --all && git reset --hard origin/main
五、团队开发避坑准则
1. 严禁在 main / master 公共主分支直接修改、提交代码
2. 每次开发前必须执行 pull 同步最新代码，规避代码冲突
3. 一个分支只对应一个功能/一个 Bug 修复，职责单一
4. 禁止随意使用 git push -f 强制推送公共分支
5. 代码冲突必须本地解决完成后，再提交合并
6. 所有 commit 备注必须清晰规范，禁止无意义提交
六、完整流程总结
环境配置 → 同步主分支代码 → 创建功能分支 → 开发调试 → add 暂存 → commit 提交 → push 推送 → 提交 PR/MR 合并 → 同步主分支 & 清理分支