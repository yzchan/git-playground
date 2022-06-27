# git rebase -i

### 问题描述：

```text
Name: reorder
Level: 48
Difficulty: ****

You have committed several times but in the wrong order. Please reorder your commits.
```

### git命令

```shell
git log --oneline // 看下顺序
git rebase -i HEAD~3
```

### 关卡解析

> 对历史commit节点进行排序，依然使用 `git rebase -i` 这个命令可以实现