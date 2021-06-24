# ignore

### 问题描述：

```text
Name: include
Level: 8
Difficulty: **

Notice a few files with the '.a' extension.  We want git to ignore all but the 'lib.a' file.
```

### git命令

```shell
echo '*.a\n' >> .gitignore
echo '!lib.a' >> .gitignore
```

### 关卡解析

> 通过.gitignore可以将一些文件加入忽略列表，使用!感叹号来添加例外文件