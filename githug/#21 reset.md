# git reset

### 问题描述：

```text
Name: reset
Level: 21
Difficulty: **

There are two files to be committed.  The goal was to add each file as a separate commit, however both were added by accident.  Unstage the file `to_commit_second.rb` using the reset command (don't commit anything).
```

### git命令

```shell
git reset HEAD to_commit_second.rb
```

### 关卡解析

> 略

### git reset 3种模式的区别

#### git reset --hard

强制回退版本，不保留回溯目标节点跟当前节点之间的所有内容。当确定不需要这些修改时可以使用hard模式。

另外如果万一回退后发现中间有些节点的内容需要找回，也是有的救的：可以通过git reflog找到回溯目标节点之后的commitId，然后再次git reset --hard <commitId>。就又回到最开始的状态了。

#### git reset --soft

同样是回退版本，但是中间被回溯版本的修改内容需要保留下来时，可以使用soft模式，回退之后git log是跟hard模式一样。只不过这些修改内容会被保留到暂存区（stage/index）。

#### git reset --mixed

跟soft模式类似，只不过修改内容会被保留到工作区，