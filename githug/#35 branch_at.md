# git branch

### 问题描述：

```text
Name: branch_at
Level: 35
Difficulty: ***

You forgot to branch at the previous commit and made a commit on top of it. Create branch test_branch at the commit before the last.
```

### git命令

```shell
git branch -f test_branch HEAD^
```

### 关卡解析

> 基于当前commit（也就是HEAD）前面的commit创建一个test_branch的分支。