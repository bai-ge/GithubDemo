# GithubDemo
git 操作实例

1.利用Android studio 创建一个工程

2.创建远程代码仓库
VCS->Import into Version Control->Share Project on Github

3.添加项目成员
setting->Contributors->Add contributor->等待对方邮件同意

4.成员建立本地仓库
VCS->Checkout from Version Control->Github->填写远程仓库URL和本地仓库路径->Clone->完成后打开工程
注意打开工程后会提示 Unregistered VCS root detected, 点击Add root
或者从Settings ->Version Control -> Directory 添加当前的工程目录

5.新建分支
右键->Git->Repository->Branches->New Branch->输入分支名称

6.切换分支
Android Studio 右下角Git选择一个本地分支
注意：切换分支之前应保证当前分支暂存区没有未提交的更改，否则切换报错
可以使用命令：
       (1)保存暂存区
       git stash save -a "tag"
       对应Android studio 右键->Git->Repository->Stash Changes->填写Message

       (2)或 提交更改
       git commit "msg"
       对应Android studio 右键->Git->Commit Directory->填写Message


7.合并分支
    对应Android studio 右键->Git->Repository->Pull->(刷新获取所有远程分支)选择一个分支进行Pull
    注意拉取完成后，需要Push更改到远程分支中

8.如果git报错403，请运行GCMW-1.14.0.exe






