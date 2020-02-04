# gitskill
1. 把GitHub网上的改动同步到本地
$ git pull origin

2. 把本地(localfile/)的改动同步到GitHub网上
$ git add localfile/
$ git cmt -m “explanation”
$ git push origin

3. 首次在本地新建文件夹(localfile/)想上传到GitHub(remotefile.git)
$ git init
$ git add localfile/
$ git cmt -m “first commit”
$ git remote add origin git@github.com:pppiao666/remotefile.git
$ git push -u origin master

4. 在GitHub上新建仓库(remotefile.git)想同步到本地文件夹(localfile/)
$ git clone git@github.com: pppiao666/remotefile.git

5. $ git cmt -am “explanation” 
-am等同于-a -m
-a参数可以将所有已跟踪文件中的执行修改或删除操作的文件都提交到本地仓库，即使它们没有经过git add添加到暂存区。
注意: 新加的文件（即没有被git系统管理的文件）是不能被提交到本地仓库的。

6. remote origin already exists.
$ git remote rm origin
$ git remote add origin git@github.com:pppiao666/remotefile.git
