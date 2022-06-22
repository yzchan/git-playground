# git stash

### 问题描述：

```text
Name: rename
Level: 14
Difficulty: ***

We have a file called `oldfile.txt`. We want to rename it to `newfile.txt` and stage this change.
```

### git命令

```shell
git mv oldfile.txt newfile.txt
```

### 关卡解析

> 跟shell用mv修改文件名一样。相当于在工作区创建newfile.txt，删除oldfile.txt，然后再提交到暂存区