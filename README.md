# git-auto-commit
使用脚本工具，实现git自动拉分支、提交代码一键完成，使用时请将git.sh文件放在当前项目的根目录，首次执行./git.sh 需先赋予权限：chmod +x git.sh

可执行命令：
1. ./git.sh 
2. ./git.sh "提交内容"
3. ./git.sh "提交内容" 单文件路径
4. ./git.sh -vm

    a. 此提交限制在dev分支中，执行此操作用于生成本次需合进master的进版内容文件并自动拉分支提交到远程。
  
    b. versions.txt记录每个版本的发版提交内容列表。
    
5.master分支禁止直接提交内容

6.如果直接在dev分支开发，执行./git.sh时会【自动新建分支】并提交到远程同名分支

7.如果已有分支上开发，执行./git.sh用于提交到远程
