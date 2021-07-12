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
> 仓库级别的配置在 .git/config 文件中。查看一下该文件：

```text
[core]
        ...
        ...
[user]
        name = ch
        email = ch@qq.com
```

查看全部配置，
```shell
git config --system --list // 系统级设置
git config --global --list // 用户级设置
git config --local --list  // 项目级设置 
git config --list
```
默认是local级。local>global>system。

```shell
git config --local user.name "username"
git config --local user.email "username@host.com"
```
在mac上 全局配置的路径为`~/.gitconfig`，项目配置的目录为`ProjectDir/.git/config`


配置git默认的编辑器
```shell
git config --global core.editor vim
git config --global core.editor emacs
```


如果遇到这个问题：
>[git]warning: LF will be replaced by CRLF in ...

一般是因为Windows和Unix/Lunix系的平台上换行符不一致引起的，只需要这么设置
```shell
git config --global core.autocrlf false
```

也有时候明明文件一模一样，git就是提示文件被修改了，多半是权限被修改导致的
```shell
git config core.filemode false
```


其他命令
```shell
git config --global color.ui true
git config --global alias.st status
```