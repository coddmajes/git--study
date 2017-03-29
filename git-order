# git--study
git使用命令-mac

 
$ mkdir repository_name//创建版本库
$ cd repository_name //查看目录
$ pwd //用于显示当前目录
$ git init //将这个目录变成Git可以管理的仓库
$ ls -ah //用于显示隐藏的目录 .git


$ git add file_name //将文件放入git仓库，注意file必须是在repository_name的目录下，实际上就是把文件修改添加到暂存区
$ git commit -m ""//将文件提交到仓库，其中“”中可以填写备注，当前提交的版本等等，实际上就是把暂存区的所有内容提交到当前分支
$ git status //查看当前仓库的状态
$ git diff //查看修改内容
$ git diff HEAD -- file_name //查看工作区和版本库里面最新版本的区别
$ git log //查看最近到最远的提交日志
$ git log --pretty=oneline //直接显示提交日志的commit_id


$ git reset --hard HEAD^ //版本回退至上一个，如果还要回退多个，即为在HEAD^后加^,如回退上上版本，即为HEAD^^，但是如果是50个版本以前，则为HEAD~50，此时情况是你还没有将你当前的本地版本推送到远程
$ git reset HEAD file_name //可以把暂存区的修改撤销掉，用HEAD表示最新的版本
$ cat file_name //查看当前文件的内容
$ git reset --hard commit_id //指定回到未来的某个版本，即当你处在本版本以前的版本时，你想回到当前版本的办法，commit_id 可以只写前面几位
$ git reflog //用于记录你的每一次命令
$ git checkout -- file_name //把文件在工作区的修改全部撤销，A，文件自修改后还没有被放到暂存区，现在，撤销修改就会到和版本库一模一样的状态；B，文件已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。总之，让这个文件回到最近一次git add 或是git commit的状态


$ rm file_name //直接删除文件，在文件管理器中
$ git rm file_name //从版本库中删除该文件，命令git rm用于删除一个文件。如果一个文件已经被提交到版本库，那么你永远不用担心误删，但是要小心，你只能恢复文件到最新版本，你会丢失最近一次提交后你修改的内容


$ git remote add origin git@github.com:XXX/repository_name.git //XXX为GitHub账户名，本地关联GitHub的远程库
$ git push -u origin master //初次把本地库的内容推送到远程，将当前分支master推送到远程，由于远程库第一次推送是空的，加上-u参数，git不但会把本地的master分支内容推送到远程新的master分支还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令
$ git push origin master //以后进行推送
$ git clone git@github.com:XXX/repository_name.git //用命令git clone克隆本地库


$ git checkout -b branch_name //git checkout命令加上-b参数表示创建并切换，相当于以下两条命令：
    $ git branch dev
    $ git checkout dev //branch代表你要创建并切换的分支名字
$ git branch //查看当前分支 显示中*表示你当前所在的分支
$ git merge branch_name //git merge命令用于合并指定分支（branch_name）到当前分支，Fast-forward，也就是直接把master指向dev的当前提交
$ git branch -d branch_name //删除当前分支


