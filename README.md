# Git命令学习

git status——查看仓库的状态
git add——向暂存区中添加⽂件
git commit——保存仓库的历史记录

git branch——显示分支
git checkout -b——创建和切换分支
git merge——合并分⽀

git reset——回溯历史版本
git reset --hard fd0cbf0d4a25f747230694d95cac1be72d33441d 
git checkout -b fix-B 

git log --graph——以图表形式查看分⽀

git log——查看提交⽇志

如果只想让程序显⽰第⼀⾏简述信息，可以在 git log 命令后加上 --pretty=short 。git diff——查看更改前后的差别
执⾏

git diff 命令，查看当前⼯作树与暂存区的差别
git diff HEAD
在执⾏ git commit 命令之前先执⾏ git diff HEAD 命令，查看本次提交与上次提交之间有什么差别，等确认完
毕后再进⾏提交。这⾥的 HEAD 是指向当前分⽀中最新⼀次提交的指
针。

接下来，我们假设 feature-A 已经实

⽤ git log --graph 命令进⾏查看的话，能很清楚地看到特性分⽀
（feature-A）提交的内容已被合并。除此以外，特性分⽀的创建以及合并
也都清楚明了。

git log 命令只能查看以当前状态为终点的历史⽇志。所以这⾥要使⽤
git reflog 命令，查看当前仓库的操作⽇志。
