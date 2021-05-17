# Git命令扩展

本文仅罗列`鲜为人知`、`很有用`的git配置或命令，不再叙述常见的Git命令。

## 设置别名

```
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
git config --global alias.last 'log -1 HEAD'
git config --global alias.logl 'log --oneline'
```

### 自动更正

该配置项只在 Git 1.6.1及以上版本有效。

如果你把help.autocorrect设置成1，那么在只有一个命令被模糊匹配到的情况下，Git 会自动运行该命令。

```
git config --global help.autocorrect 1
```

### 忽略大小写

Git 默认是忽略大小写的

```
git config core.ignorecase false
git config core.ignorecase true
```