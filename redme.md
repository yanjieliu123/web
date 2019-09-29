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
