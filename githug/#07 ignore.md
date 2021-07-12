# ignore

### 问题描述：

```text
Name: ignore
Level: 7
Difficulty: **

The text editor 'vim' creates files ending in `.swp` (swap files) for all files that are currently open.  We don't want them creeping into the repository.  Make this repository ignore those swap files which are ending in `.swp`.
```

### git命令

```shell
echo '*.swp' >> .gitignore
```

### 关卡解析

> 总有一些文件是不需要进行版本管理的，比如代码执行过程中的临时文件，或者带敏感数据的配置文件等等。通过.gitignore可以将这些文件加入忽略列表，git就不会管理到这些文件了。