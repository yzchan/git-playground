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
git checkout new-feature
git log --oneline # 找到需要保留的节点commit id
# ea2a47c (HEAD -> new-feature) some small fixes
# 4a1961b Fixed feature
# ca32a6d Filled in README.md with proper input
# 58a8c8e Added a stub for the feature
# ea3dbcc Initial commit
git checkout master
git cherry-pick ca32a6d
```

### 关卡解析

> 抓取某些节点的修改，这个命令使用十分方便。