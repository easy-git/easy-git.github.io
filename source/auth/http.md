---
date: 2021-01-09 22:19:35
---

## Windows: 在 Git 中缓存凭据

如果您 使用 `HTTPS` 克隆 Git 仓库，您可以使用凭据小助手告诉 Git 记住您的凭据。

使用 Windows 版 Git 时，在命令行中运行以下内容将存储凭据：

```
$ git config --global credential.helper wincred
```

##### Windows: 凭据管理器

在Windows电脑，开始菜单，搜索`凭据管理器`，找到后，点击打开。

在`凭据管理器`窗口，您可以`添加凭据`、或删除已有凭据。

<div style="text-align: center;">
    <img src="/static/wincred.png" />
</div>