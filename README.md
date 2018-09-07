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

##### delete native

```shell
git branch -d <branchname>
```

##### delete romote

```shell
git branch -r -d origin/<branchname>
git push origin :<branchname>
```

##### list all native branch

```shell
git branch
```

##### list all remote branch

```shell
git branch -r
```



####clone

#####clone project

```shell
git clone https://github.com/wyhazq/GitCommand.git
```



#### commit

##### commit to native with modify info

```shell
//1
git add .
git commit -m 'modify info'

//2
git commit -am 'modify info'
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



#### diff

##### work & native diff

```shell
git diff
```

##### native & remote diff

```shell
git diff --cached
```

##### both

```shell
git diff HEAD
```

##### short diff

```shell
git diff --stat
```



#### log

#####all log

```
git log
```

#####short log

```
git log --oneline
```

##### graph log 

```shell
git log --oneline --graph
```

#####reverse log

```shell
git log --reverse
```

##### author log

```
git log --author=<username>
```

##### time log

```
git log --before={3.weeks.ago} --after={2008-08=08}
```

##### no merge log

```
git log --no-merges
```





#### merge

```shell
git merge <branchname>
```



#### mv

```shell
git mv <filename> <new filename>
```



#### pull

```shell
git pull origin
```



#### push

#####push current branch

```shell
git push origin
```

##### push a branch

```shell
git push origin <branchname>
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



#### status

##### short status

```shell
git status -s
```

##### all status

```shell
git status
```



#### tag

##### add native tag

```shell
git tag -a <tagname> -m 'modify info'
```

#####delete native tag

```shell
git tag -d <tagname>
```

##### delete remote tag

```
git push
```



##### list tags

```shell
git tag
```

##### push tag

```
git push origin <tagname>
```





#### change git history author info

[change git history author info](https://help.github.com/articles/changing-author-info/)



















