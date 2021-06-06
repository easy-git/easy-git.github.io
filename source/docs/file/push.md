---
date: 2021-01-10 12:01:35
---

## git push 推送

git push: 用于将本地分支的更新，推送到远程。

easy-git插件中，执行pull操作的方式：

- 源代码管理器视图，点击底部的`上箭头 ↑`。
- 命令面板，输入`push`。 [关于命令面板](/CommandPanel)

注意：push的前提是，本地已关联远程仓库。

## 命令面板

easy-git插件，命令面板，提供了关于push的各种选项操作，

- `git push`
- `git push --force` : 强制推送
- `git push --force-with-lease` : 安全性的强制推送
- `git push --no-verify` : 绕过验证推送


如下截图：

<img src="/static/commandpanel-push.png" style="border: 1px solid #eee;" />