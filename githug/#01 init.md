# git init

### 问题描述：

```text
Name: init
Level: 1
Difficulty: *

A new directory, `git_hug`, has been created; initialize an empty repository in it.
```

### git命令

```shell
git init
```

> git对于版本的一切管理都从git init初始化仓库开始。git init会在当前目录创建.git目录，版本管理相关的记录都在里面。如果不需要对当前目录进行版本管理了，删除.git目录即可。
> git是一个分布式版本管理工具。把代码推送到远端是基于数据备份和多人协作的需求。如果不考虑远端，仅仅在本机使用git进行版本管理依然可以体验到git强大的功能。
