# reader 文档
- 项目说明文档
- 一般都与项目放在一起

# git操作

## 初始化版本库
- git init
- 初始化成功后，当前目录后面有(master)
- 初始化成功后当前目录下有个隐藏文件.git(不要管，不要操作这个文件)

## 工作区
- 持有实际文件
- 我们平时增删改查的文件都是工作区的内容

## 提交到暂存区
- 可以理解为我们看不到的一个地方
- 也是存在于用户电脑中的
- 本地仓库的一个主要组成部分

## 本地仓库
- 可以理解为我们看不到的一个地方
- 也是存在于用户电脑中的
- 用于存储项目代码及版本项目记录等信息

## 提交到暂存区
- git add 文件名
- 将工作区的变动提交到暂存区
- git add . 将所有变动提交到暂存区

## 查看状态
- git status
- 查看工作区和暂存区的状态（增删改）

## 提交到本地仓库
- git commit -m '提交注释'
- 将代码从暂存区提交到本地仓库
- git status 查看状态提示：工作区是干净的，没有任何东西需要提交

## 本地操作关键步骤
1. git init (只有第一次需要操作，有.git文件夹的时候就不要操作了)
2. git add .
3. git commit -m '注释'
4. git status 
  查看工作区和暂存区状态（增删改查）

## 查看日志
- git log  完整版日志
- git reflog  简单版日志

## 版本回退
- git reset --hard HEAD^  回退到
- git reset --hard 版本号前7位数
- 注意把当前代码先提交到本地仓库
- 工作区的代码自动变成恢复的指定版本

## 查看变动
- git diff 文件名
- 会列出该文件前后的差异

## 创建远程仓库
- 进入gitHub官网，创建一个新的远程仓库

## 将本地仓库和远程仓库关联
- git remote add origin https://github.com/a646757947/GP5.git   (后面这个地址就是自己的远程仓库地址)