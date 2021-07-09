# git stage

### 问题描述：

```text
Name: stage_lines
Level: 50
Difficulty: ****

You've made changes within a single file that belong to two different features, but neither of the changes are yet staged. Stage only the changes belonging to the first feature.
```

### git命令

```shell
git add feature.rb --edit // vim中删除最后一行即可
```

### 关卡解析

> 只提交同一个文件中的部分代码。不常用