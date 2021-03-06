# Learn Git

## Basic
**Git教程:** 引用
https://www.liaoxuefeng.com/wiki/896043488029600
### Useful Code

`git init`

`git add .//把文件添加到仓库`

`git commit -m "文本"`

`git status//掌握仓库当前的状态`

`git diff`

`git log/*git log --pretty=oneline*/`

```
git reset --hard HEAD^//回退到上一版本
/*上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100*/
```

*HEAD相当于一个指针,指向的版本就是当前版本*

未来版本需要使用commit id

`cat .`

`git reflog//用来记录你的每一次命令`

Git管理是保存修改，所以每次都要进行`add`与`commit`操作

`git diff HEAD -- readme.txt//查看工作区和版本库里面最新版本的区别`

`git checkout -- file//可以丢弃工作区的修`

`git reset HEAD <file>//可以把暂存区的修改撤销掉（unstage），重新放回工作区`

`git rm file//delete`
一是确实要从版本库中删除该文件，那就用命令`git rm`删掉，并且`git commit`

`git remote add origin git@`

`git push -u origin master`

`git push origin master//从现在起，只要本地作了提交，就可以通过命令`

如果添加的时候地址写错了，或者就是想删除远程库，可以用`git remote rm <name>`命令。使用前，建议先用`git remote -v`查看远程库信息：

## Q&A

**fatal: remote origin already exists. (远程来源已经存在 解决办法):**
https://cloud.tencent.com/developer/article/1880265

**使用 vscode将本地项目上传到github、从github克隆项目以及删除github上的某个文件夹:**
https://www.cnblogs.com/lihuijuan/p/8556914.html
