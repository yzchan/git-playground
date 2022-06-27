# git merge

### 问题描述：

```text
Name: merge_squash
Level: 47
Difficulty: ***

Merge all commits from the long-feature-branch as a single commit.
```

### git命令

```shell
git merge long-feature-branch --squash
git commit -m"."
```

### 关卡解析

> 当我们从其他分支merge到主分支时，通常会带来大量的commit，如果我们不希望一个Merge Request产生这么多的commit，可以在merge时带上--squash选项。