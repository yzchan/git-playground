git rebase
-----

合并commit，让提交历史更加整洁：
```shell
git rebase -i HEAD~5  // 合并最近5次commit  pick => squid
git push -f // 当需要合并的commit已经再远端时 需要git push -f 强制更新远端 
```

> git push -f 命令需要慎用。如果只有自己使用仓库就无所谓，如果是多人合作尤其要慎用。

其他协作者需要使用使用 git reset --hard origin/master 来强制本地分支跟线上保持一致。如果有尚未提交的修改可以配合git stash先暂存。
