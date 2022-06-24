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
git branch -d delete_me  # 删除一个名字为branchName的分支。如果该分支有提交未进行合并，则会删除失败。
git branch -D delete_me  # 强制删除一个名字为branchName 的分支。如果该分支有提交未进行合并，也会删除成功。

```

### 关卡解析

> 删除分支