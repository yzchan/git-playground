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

> 依旧是git rebase -i HEAD~3 之后调整顺序保存即可