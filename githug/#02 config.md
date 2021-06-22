# git config

### 问题描述：

```text
Name: config
Level: 2
Difficulty: *

Set up your git name and email, this is important so that your commits can be identified.
```

### git命令

```shell
git config --local user.name ch
git config --local user.email ch@qq.com
```

### 返回结果

```text
What is your name? ch
What is your email? ch@qq.com
Your config has the following name: ch
Your config has the following email: ch@qq.com
Congratulations, you have solved the level!
```

### 关卡解析

> 设置用户配置。这里使用的是--local仓库级别的设置。也可以使用[--global]全局级别设置或者[--system]系统级别设置。
> 仓库级别的配置会卸载 .git/config 文件中。查看一下该文件：

```text
[core]
        ...
        ...
[user]
        name = ch
        email = ch@qq.com
```