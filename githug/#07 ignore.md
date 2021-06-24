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

> 通过.gitignore可以将一些文件加入忽略列表