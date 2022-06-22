# git stash

### 问题描述：

```text
Name: stash
Level: 13
Difficulty: **

You've made some changes and want to work on them later. You should save them, but don't commit them.
```

### git命令

```shell
git stash
```

### 关卡解析

> 功能做了一半暂时不想提交，又必须要切换分支时可以使用git stash将修改暂存到堆栈中。切完分支回来还可以从堆栈中弹出来。

### 常用git stash命令：

- git stash save "save message"  : 执行存储时，添加备注，方便查找，只有git stash 也要可以的，但查找时不方便识别。
- git stash list  ：查看stash了哪些存储
- git stash show ：显示做了哪些改动，默认show第一个存储,如果要显示其他存贮，后面加stash@{$num}，比如第二个 git stash show stash@{1}
- git stash show -p : 显示第一个存储的改动，如果想显示其他存存储，命令：git stash show  stash@{$num}  -p ，比如第二个：git stash show  stash@{1}  -p
- git stash apply :应用某个存储,但不会把存储从存储列表中删除，默认使用第一个存储,即stash@{0}，如果要使用其他个，git stash apply stash@{$num} ， 比如第二个：git stash apply stash@{1}
- git stash pop ：命令恢复之前缓存的工作目录，将缓存堆栈中的对应stash删除，并将对应修改应用到当前的工作目录下,默认为第一个stash,即stash@{0}，如果要应用并删除其他stash，命令：git stash pop stash@{$num} ，比如应用并删除第二个：git stash pop stash@{1}
- git stash drop stash@{$num} ：丢弃stash@{$num}存储，从列表中删除这个存储
- git stash clear ：删除所有缓存的stash