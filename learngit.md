# learngit

### 1.创建版本库

```
mkdir learngit
cd learngit/
pwd
/Users/zhuyun/Desktop/Project/learngit
git init
```

### 2.在git仓库中创建一个txt文件

```
readme.txt
git add readme.txt
```

### 3.提交文件到仓库

```
git commit -m "wrote a readme file"
```

### 4.显示从最近到最远的提交日志

```
git log
git log --pretty=oneline
```

### 5.版本回退

```
git reset --hard HEAD^
```

### 6.到达指定版本

```
git reset --hard f12ec
```

### 7.查看命令执行记录

```
git reflog
```

### 8.撤销工作区的修改

```
git checkout -- readme.txt
```

### 9.删除文件

```
git rm test.txt
```

### 10.本地git库链接远程仓库

```
git remote add origin git@github.com:cj1234567/learngit.git
```

### 11.本地内容推送到远程仓库

```
git push -u origin master
```

### 12.生成git密钥

```
ssh-keygen -t rsa -C "515517617@qq.com"
```

### 13.添加私密钥到ssh

```
ssh-add id_rsa
```

### 14.添加公钥到github

```
a、首先你需要拷贝 id_rsa.pub 文件的内容，你可以用编辑器打开文件复制，也可以用git命令复制该文件的内容，如：
b、登录你的github账号，从又上角的设置（ Account Settings ）进入，然后点击菜单栏的 SSH key 进入页面添加 SSH key。
c、点击 Add SSH key 按钮添加一个 SSH key 。把你复制的 SSH key 代码粘贴到 key 所对应的输入框中，记得 SSH key 代码的前后不要留有空格或者回车。当然，上面的 Title 所对应的输入框你也可以输入一个该 SSH key 显示在 github 上的一个别名。默认的会使用你的邮件名称。
```

### 15.远程仓库拉去到本地

```
git pull --rebase https://github.com/cj1234567/learngit.git master
```

### 16.创建dev分支git branch dev，然后切换到dev分支git checkout dev

```
git checkout -b dev -b参数表示创建并切换
git branch命令会列出所有分支，当前分支前面会标一个*号。
```

### 17.切换分支

```
git checkout master
```

### 18.合并分支

```
git merge <name>
```

### 19.删除分支

```
git branch -d <name>
```

### 20.查看分支

```
git branch
```


### 21创建分支

```
git branch <name>
```


### 22创建+切换分支

```
git checkout -b <name>
```


