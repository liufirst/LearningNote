# 与github库进行连接
①首先在本地创建文件夹（总库）

②执行`git  clone  https://github.com/liufirst/LearningNote.git`命令，拷贝仓库到“本地总库”

③执行`git init`将clone下的文件夹初始化

④接着是常规的`git add ****`、`git  commit -m"***" `

⑤如果是克隆来的话，其实默认已经将本地文件夹和github上的仓库连接了，不需要`git remote add origin https://github.com/liufirst/LearningNote.git`,此命令就是为了链接网上仓库

⑥`git push origin master`命令，将本地仓库的文件推送到网上仓库。关于这个地方， **有个地方需要注意！！** 

在我们向远程仓库提交代码的时候，一定要先进行`pull`操作，再进行`push`操作，防止本地仓库与远程仓库不同步导致冲突的问题，尤其是第二种提交代码的情况，很容易就出现问题。