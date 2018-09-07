# GitCommand

[Git 工作区、暂存区和版本库](http://www.runoob.com/git/git-workspace-index-repo.html)

#### add

##### add all files

```shell
git add .
```

##### add some files

```shell
git add <file>...
```



#### branch

##### create

```shell
git branch <branchname>
```

##### create & checkout Immediately

```shell
git checkout -b <branchname>
```

##### checkout

```shell
git checkout <branchname>
```

##### delete

```shell
git branch -d <branchname>
```

##### list all branch

```shell
git branch
```



####clone

#####clone project

```shell
git clone https://github.com/wyhazq/GitCommand.git
```



#### config

##### global userInfo

```shell
git config --global user.name 'username'
git config --global user.email test@github.com
```

##### current git userInfo

```shell
git config -f .git/config user.name 'username'
git config -f .git/config user.email test@github.com
```



#### merge

```shell
git merge <branchname>
```







#### status

#####short status

```shell
git status -s
```

#####all status

```shell
git status
```





#### diff

#####work & native diff

```shell
git diff
```

#####native & remote diff

```shell
git diff --cached
```

#####both

```shell
git diff HEAD
```

#####short diff

```shell
git diff --stat
```





#### commit

#####commit to native with modify info

```shell
//1
git add .
git commit -m 'modify info'

//2
git commit -am 'modify info'
```







#### push

```shell
git push origin master
```



#### reset

#####cancel cached file

```shell
git reset HEAD <file>
```

#####cancel last commit

```shell
git reset HEAD^
```



#### rm

#####remove work file

```shell
git rm <file>
```

##### remove work & native file

```shell
git rm -f <file>
```

##### remove native file

```shell
git rm --cached <file>
```

#####remove all file

```shell
git rm –r * 
```



#### mv

```shell
git mv <filename> <new filename>
```



