# git rm

### 问题描述：

```text
Name: rm_cached
Level: 12
Difficulty: **

A file has accidentally been added to your staging area, find out which file and remove it from the staging area.  *NOTE* Do not remove the file from the file system, only from git.
```

### git命令

```shell
git rm --cached deleteme.rb
```

### 关卡解析

> git rm --cached删除暂存区和版本库的文件，但保留了工作区的文件