# git restore

### 问题描述：

```text
Name: restore
Level: 53
Difficulty: ****

You decided to delete your latest commit by running `git reset --hard HEAD^`.  (Not a smart thing to do.)  You then change your mind, and want that commit back.  Restore the deleted commit.
```

### git命令

```shell
git reflog // 查看操作记录  找到需要restore的commit id
git reset --hard 137e632
```

### 关卡解析

> 