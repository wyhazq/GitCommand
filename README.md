# GitCommand

### 4 space: *work* *cache* *native* *remote*

## Directory

##### [add](#add)

##### [branch](#branch)

##### [checkout](#checkout)

##### [clone](#clone)

##### [commit](#commit)

##### [config](#config)

##### [diff](#diff)

##### [fetch](#fetch)

##### [log](#log)

##### [merge](#merge)

##### [mv](#mv)

##### [pull](#pull)

##### [push](#push)

##### [rm](#rm)

##### [remote](#remote)

##### [reset](#reset)

##### [status](#status)

##### [tag](#tag)

##### [change git history author info](#change-git-history-author-info)



#### add

##### add all files to cache

```shell
git add .
```

##### add some files to cache

```shell
git add <file>...
```



#### branch

##### create

```shell
git branch <branchname>
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



#### checkout

##### create & checkout Immediately

```shell
git checkout -b <branchname>
```

##### checkout

```shell
git checkout <branchname>
```

##### discard changes

```shell
git checkout -- <file>
```



#### clone

##### clone project

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

##### current git userInfo

```shell
git config -f .git/config user.name 'username'
git config -f .git/config user.email test@github.com
```

##### global userInfo

```shell
git config --global user.name 'username'
git config --global user.email test@github.com
```

##### list config

```shell
git config --list
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

##### both diff

```shell
git diff HEAD
```

##### short diff

```shell
git diff --stat
```



#### fetch

##### all update

```shell
git fetch
```

##### current branch

```shell
git fetch origin
```

##### a branch

```shell
git fetch origin <branchname>
```



#### log

##### all log

```
git log
```

##### short log

```
git log --oneline
```

##### graph log 

```shell
git log --oneline --graph
```

##### reverse log

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

##### push current branch

```shell
git push origin
```

##### push a branch

```shell
git push origin <branchname>
```



#### rm

##### remove work file

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

##### remove all file

```shell
git rm –r * 
```



#### remote

##### remote info

```shell
git remote -v
```



#### reset

##### reset all cache file to work

```shell
git reset .
```

##### reset cache file to work

```shell
git reset <file>
```

##### cancel last commit

```shell
git reset --hard HEAD^
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

##### delete native tag

```shell
git tag -d <tagname>
```

##### delete remote tag

```
git push origin :refs/tags/<tagname>
```



##### list tags

```shell
git tag
```

##### push tag

```
//1
git push origin <tagname>
//2
git push --tags
```





#### change git history author info

[change git history author info](https://help.github.com/articles/changing-author-info/)

