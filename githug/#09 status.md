# git status

### 问题描述：

```text
Name: status
Level: 9
Difficulty: *

There are some files in this repository, one of the files is untracked, which file is it?
```

### git命令

```shell
What is the full file name of the untracked file? database.yml
```

### 关卡解析

> git status查看状态
> - Changes to be committed: git add 过的文件
> - Changes not staged for commit: 版本中已经有文件，但是修改过。
> - Untracked files :还有添加到版本的文件。
