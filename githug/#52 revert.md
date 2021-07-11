# git revert

### 问题描述：

```text
Name: revert
Level: 52
Difficulty: ****

You have committed several times but want to undo the middle commit.
All commits have been pushed, so you can't change existing history.
```

### git命令

```shell
git log --oneline //查看错误分支名
git revert 563832f // 选择刚才看到的分支名
```

### 关卡解析

> git reset是回退到过去的commit,后面的commit就被放弃了。git revert是重做，会创建一个新的commit，同时也会保留有问题的commit之后的所有commit。