git init 初始化仓库
git add <file>  添加文件可反复使用, 可同时添加多个文件
git commit -m '此次提交的版本注释' 将添加的文件提交到仓库
git status 查看仓库当前状态,比如修改了文件却没有提交, 告诉你有文件被修改过
git diff 查看未提交文件变化情况,可以查看修改内容。
git log 修改记录,各版本修改记录
git log --pretty=oneline 将各版本修改记录一行显示
git reset hard HEAD^ HEAD代表当前版本, HEAD^表示上一个版本, 上上个版本可以写成HEAD^^, 上100个版本可以写成HEAD~100
git reset hard 版本号   回退到某一个版本,版本号只需要填写前面几个即可
git reflog 记录命令记录,可以找到某个版本的版本号,可用作恢复等操作
cat 文件   查看文件内容
git checkout -- 文件   把文件在工作区的修改全部撤销一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。总之，就是让这个文件回到最近一次git commit或git add时的状态。
git reset HEAD file   将add到暂存区的文件撤销.回复到最新版本
git rm file   删除一个文件
git push origin master  同步到GitHub仓库