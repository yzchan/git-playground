# git cherry-pick

### 问题描述：

```text
Name: cherry-pick
Level: 43
Difficulty: ***

Your new feature isn't worth the time and you're going to delete it. But it has one commit that fills in `README` file, and you want this commit to be on the master as well.
```

### git命令

```shell
git cherry-pick ca32a6d
```

### 关卡解析

> 先在new-feature分支上找到需要pick的commit_id