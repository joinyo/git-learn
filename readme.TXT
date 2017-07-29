1.git 是一种分布式版本管理工具

2.基础命令

git add 命令:工作区增加到暂存区
git commit 命令：暂存区提交到版本库（对象库）中

git checkout HEAD . 或 git checkout HEAD <file> 命令：版本库替换暂存区和工作区中的文件
git reset HEAD 命令：版本库替换暂存区的文件
git checkout . 或 git checkout -- <file> 命令：暂存区替换工作区的文件

git rm <file>  删除缓存区和工作区的文件
git rm --cached <file> 删除缓存区文件

git mv old_name  new_name   对暂存区重命名

3.将Windows本地文件上传到github的操作

a)安装git

b)在文件夹内（工作区/工作空间）里右键——Git Bash Here ,在弹出的MINGW64中输入git init 
c)再在弹出的MINGW64中输入ssh-keygen -t rsa -C "github.com上注册的邮箱"
方便起见，默认密码为空，即一直按enter键即可。
###注意ssh-keygen命令中间没有空格，如果在ssh后面加上空格，会得到Bad escape character 'ygen'.的错误。

d)Add SSH，key为.ssh文件夹下的id_rsa.pub内容(C:\Users\Administrator\.ssh\id_rsa.pub)

e)创建repository

f)连接仓库，上传文件 git remote add origin https://github.com/joinyo/git-learn.git

3.配置
#git config --global user.name  "姓名"
#git config --global user.email  "邮箱"
