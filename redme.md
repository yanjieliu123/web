配置用户名
$ git config --global user.name "LYJ"
配置邮箱
$ git config --global user.email "yanjie_liu123@163com"


提交文件命令 分两步
$ git add redme.md

$ git commit -m "git基本配置使用命令"

多个文件操作
$ git add ./
$ git commit --all -m "多文件存放说明"

查看日志

$ git log 显示所有详细信息
git log --oneline 显示单行提交内容

返回旧版本
$ git reset --hard HEAD~0  （数字0可以为1或者更大，回退版本更早）

通过版本号切换版本

git reset --hard "具体版本号" （不用双引号）

git reset --hard [版本号]

切换到旧版本后原来的版本号怎么查看？

git reflog
可以查看版本切换记录

创建分支与分支切换
git branch [name]

git branch 命令查看所有分支

git checkout [name]

合并分支
git merge [name]

删除分支
git branch -d [name]


两个并行分支分别开发不同功能后合并问题，怎么做到两者功能合并？
手动改变两份之代码后才能兼并否则无法合并



团队开发代码，如何共享项目代码？

使用GItHub，允许通过git上传代码的功能
https://github.com/yanjieliu123/web.git我的个人账户

$ git push https://github.com/yanjieliu123/web.git master
上传到github仓库


$ git pull https://github.com/yanjieliu123/web.git master
获取GITHub服务器仓库文件，需要提前git init本地库

在push和pull操作时首先pull操作下载文件到本地，然后再进行push操作

push和pull操作简写：
通过如下
git remote add origin https://github.com/yanjieliu123/web.git
定义 origin,可以用 origin替代远程连接地址

第一次使用
git clone [远程路径]会自动创建本地仓储

##使用ssh方式上传代码
-公钥 私钥，两者之间有关联；私钥自留，公钥可以团队内部使用。
-生成公钥和私钥
 +生成命令：$ ssh-keygen -t rsa -C "yanjie_liu123@163.com"



