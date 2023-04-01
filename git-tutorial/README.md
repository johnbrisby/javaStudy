## 这是一些基础的常用git命令
### 1.Git上创建项目，本质上就是创建一个仓库(Repository)，不需要启动什么server，只要命启动令行，切到自己项目文件夹的根目录下，运行命令：

>git init

### 2.克隆（Clone）项目
>git clone https://github.com/username/demo-repo.git
### 2.远程remote项目
>git remote add origin git@

### 3.提交（commit）代码
git add .

git commit -m "some comments for this commit"

参数“-m” 后面跟的是当前提交的备注。

### 4.推送（Push）代码
git push
什么时候可以push呢？就是在已经commit过就可以push了

### 5.拉取（Pull）代码
git pull

### 6.创建分支（branch）
git branch testing      创建一个 testing 分支，需要使用 git branch 命令：

git checkout testing    切换 分支

git branch              查看所有分支，会列出所有本地的分支，但不包括远程的分支。

git branch -a           要查看本地和远程分支，可以加上-a参数：

### ssk  官网指南https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
>ssh-keygen -t rsa -b 4096 -C “------@gmail.com”

>Enter file in which to save the key (/Users/---/.ssh/id_rsa): mainkey

>% ls | grep mainkey
用grep快速找出mainkey的文件

 cat mainkey.pub   |  pbcopy < ~/testkey.pub  ----- 复制txt到github 

 vim ~/.ssh/config

 If the file doesn't exist, create the file.

>$ touch ~/.ssh/config

  Host github.com

  AddKeysToAgent yes

  UseKeychain yes

  IdentityFile ~/.ssh/id_rsa


 >ssh-add -K ~/.ssh/id_rsa


 