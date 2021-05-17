---
date: 2021-01-09 22:19:35
---

# 分支切换

源代码管理器视图，底部**分支名称**：

- 鼠标`左键`，点击打开`分支管理视图`
- 鼠标`右键`、`中键`，点击直接切换到`上一个分支`

<div style="margin: 1rem;">
    <img src="/static/branch-switch.png" />
</div>


## 通过命令面板切换分支

打开【命令面板】，搜索：`分支切换`

## Git 命令: 切换分支

```bash
$ git switch <branch-name>      // 切换到指定分支
$ git checkout -                // 切换到上个分支

$ git checkout <branch-name>          
```

说明：`git checkout`和`git switch`都可以实现切换分支的功能

## git switch来源

`git checkout`命令承载了分支操作和文件恢复的部分功能，有点复杂，并且难以使用和学习。

所以Git社区将这两部分功能拆分开，在git `2.23.0`中引入了新的命令`switch`