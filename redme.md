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
获取GITHub服务器仓库文件




