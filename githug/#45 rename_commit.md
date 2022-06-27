# git grep

### 问题描述：

```text
Name: rename_commit
Level: 45
Difficulty: ***

Correct the typo in the message of your first (non-root) commit.
```

### git命令

```shell
git rebase -i HEAD~2
# 将First coommit前面的pick改成reword
# 保存后进入第二个vim界面，修改错误内容，保存退出。
```

### 关卡解析

> git rebase -i 可以修改历史节点。如果只需要修改上一次提交的commit信息也可以使用 `git commit --amend`