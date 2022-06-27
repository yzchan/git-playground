# git rebase

### 问题描述：

```text
Name: squash
Level: 46
Difficulty: ****

You have committed several times but would like all those changes to be one commit.
```

### git命令

```shell
git rebase -i HEAD~4
# 第一个vim修改界面，将需要合并的3个commit前面的pick改成squash
# 保存后进入第二个vim界面，填写新的commit备注，保存退出。
```

### 关卡解析

> git rebase -i HEAD~4之后进入