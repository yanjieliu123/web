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