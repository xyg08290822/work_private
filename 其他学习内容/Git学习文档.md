# Git学习文档

## Git简介

Git是一个开源的分布式版本控制系统，用于高效地处理任何大小项目的版本管理。

Git是Linus Torvalds为了帮助管理Linux内核开发而开发的一个开放源码的版本控制软件。

Git与常用的版本控制工具CVS、Subversion等不同，它采用了分布式版本库的方式，不必服务器端软件支持。

## Git安装

### Windows安装

1. 下载Git安装包，可以从Git官网下载，也可以从其他可靠的源下载。

2. 运行安装包，按照安装向导的提示进行安装。

3. 安装完成后，打开命令行工具，输入`git --version`，如果能够正确显示Git的版本号，则说明安装成功。

### Linux安装

1. 打开终端，输入以下命令：

   ```
   sudo apt-get install git
   ```

2. 等待安装完成，输入以下命令：

   ```
   git --version
   ```

3. 如果能够正确显示Git的版本号，则说明安装成功。

## Git基本命令

### 配置用户信息

1. 配置用户名：

   ```  bash
   git config --global user.name "Your Name"
   ```

2. 配置用户邮箱：

   ```bash
   git config --global user.email "your_email@example.com"
   ```

### 初始化仓库

1. 在命令行中进入要初始化的目录，输入以下命令：

   ```bash
   git init
   ```

2. 初始化完成后，该目录下会生成一个名为`.git`的隐藏文件夹，这就是Git的版本库。

### 添加文件

1. 在命令行中进入要添加文件的目录，输入以下命令：

   ```bash
   git add <file>
   ```

2. 可以使用通配符`*`来添加所有文件，例如：

   ```bash
   git add *
   ```

### 提交更改

1. 在命令行中输入以下命令：
    ```bash
    git commit -m "commit message"
    ```

### 查看状态

1. 在命令行中输入以下命令：

   ```bash
   git status
   ```

2. 该命令会显示当前仓库的状态，包括未跟踪的文件、已修改的文件等。

### 查看日志

1. 在命令行中输入以下命令：

   ```bash
   git log
   ```

2. 该命令会显示提交的日志，包括提交的哈希值、提交者、提交时间、提交信息等。

### 查看差异

1. 在命令行中输入以下命令：

   ```bash
   git diff
   ```

2. 该命令会显示工作目录和暂存区之间的差异。

### 回滚到指定版本

1. 在命令行中输入以下命令：

   ```bash
   git reset --hard <commit_hash>
   ```

2. 该命令会回滚到指定版本的提交。

### 删除文件
1. 在命令行中输入以下命令：
    ```bash
    git rm <file>
    ```

### 克隆仓库

1. 在命令行中输入以下命令：

   ```bash
   git clone <repository_url>
   ```

2. 该命令会克隆指定URL的仓库到当前目录。

### 分支管理

1. 创建分支：

   ```bash
   git branch <branch_name>
   ```
2. 切换分支：

   ```bash
   git checkout <branch_name>
   ```
3. 合并分支：

   ```bash
   git merge <branch_name>
   ```
4. 删除分支：

   ```bash
   git branch -d <branch_name>
   ```
5. 创建新分支并直接切换到这个新分支：
   ```bash
   git checkout -b <branch_name>
   ```

### 远程仓库管理

1. 添加远程仓库：

   ```bash
   git remote add <remote_name> <repository_url>
   ```
2. 查看远程仓库：

   ```bash
   git remote -v
   ```
3. 推送本地分支到远程仓库：

   ```bash

   git push <remote_name> <branch_name>
   ```
4. 拉取远程仓库的更新：

   ```bash
   git pull <remote_name> <branch_name>
   ```

### 标签管理

1. 添加标签：

   ```bash
   git tag <tag_name>
   ```
2. 查看标签：

   ```bash
   git tag
   ```
3. 删除标签：

   ```bash
   git tag -d <tag_name>
   ```
4. 推送标签到远程仓库：

   ```bash
   git push <remote_name> <tag_name>
   ```

### 代码审查

1. 查看提交历史：

   ```bash
   git log
   ```
2. 查看提交差异：

   ```bash
   git diff <commit_hash1> <commit_hash2>
   ```
3. 查看提交信息：

   ```bash
   git show <commit_hash>
   ```
4. 查看分支信息：

   ```bash
   git branch -v
   ```
5. 查看远程分支信息：

   ```bash
   git branch -r
   ```

### 其他命令

1. 查看当前分支：

   ```bash
   git branch
   ```
2. 查看当前分支的提交历史：

   ```bash
   git log
   ```
3. 查看当前分支的提交差异：

   ```bash
   git diff
   ```
4. 查看当前分支的提交信息：

   ```bash
   git show
   ```
5. 查看当前分支的分支信息：

   ```bash
   git branch -v
   ```
6. 查看当前分支的远程分支信息：

   ```bash
   git branch -r
   ```
7. 查看当前分支的标签信息：

   ```bash
   git tag
   ```
8. 查看当前分支的远程仓库信息：

   ```bash
   git remote -v
   ```
