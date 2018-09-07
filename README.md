# GitCommand

[Git 工作区、暂存区和版本库](http://www.runoob.com/git/git-workspace-index-repo.html)

#### add

##### add some files

```shell
git add <file>...
```

##### add all files

```shell
git add .
```



#### branch

##### create

```shell
git branch <branchname>
```

##### switch

```shell
git checkout <branchname>
```









####clone

#####clone project

```shell
git clone https://github.com/wyhazq/GitCommand.git
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



#### config

#####global userInfo

```shell
git config --global user.name 'userName'
git config --global user.email test@github.com
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



