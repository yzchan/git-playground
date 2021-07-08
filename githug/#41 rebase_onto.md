# git rebase

### 问题描述：

```text
Name: rebase_onto
Level: 41
Difficulty: **

You have created your branch from `wrong_branch` and already made some commits, and you realise that you needed to create your branch from `master`. Rebase your commits onto `master` branch so that you don't have `wrong_branch` commits.
```

### git命令

```shell
git rebase -i wrong_branch
// 然后将第一行(即有错误的那个commit)前面的pick改成drop 然后保存即可
```

### 关卡解析

> git rebase -i 可以对历史commit进行选取、丢弃、排序等，十分强大。