---
date: 2021-01-09 22:19:35
---

# git pull

Git pull: 从远端仓库中抓取数据，合并到工作目录中的当前分支。

easy-git插件中，执行pull操作的方式：

- 源代码管理器视图，点击底部的`下箭头 ↓`。注意：此处运行的git命令为：`git pull --rebase`
- 命令面板，输入`pull`。 [关于命令面板](/CommandPanel)

## 命令面板

easy-git插件，命令面板，提供了关于pull的各种选项操作，

- git pull
- git pull --rebase
- git pull --rebase --autostash

如下截图：

<img src="/static/commandpanel-pull.png" style="border: 1px solid #eee;" />


> 使用下面的关系，简单的说明下 git pull和git pull --rebase的区别：

```
git pull = git fetch + git merge
git pull --rebase = git fetch + git rebase
```