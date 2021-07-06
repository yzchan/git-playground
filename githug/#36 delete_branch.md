# git branch

### 问题描述：

```text
Name: delete_branch
Level: 36
Difficulty: **

You have created too many branches for your project. There is an old branch in your repo called 'delete_me', you should delete it.
```

### git命令

```shell
git branch -d delete_me
```

### 关卡解析

> 基于当前commit（也就是HEAD）前面的commit创建一个test_branch的分支。