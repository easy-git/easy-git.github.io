---
date: 2021-01-15 22:19:35
---

# 弹出储藏

> git stash pop， 弹出储藏， 可以恢复之前缓存的工作目录。

## 如何使用？

- easy-git源代码管理器视图，点击顶部菜单【...】，点击【弹出最新储藏】
- easy-git源代码管理器视图，点击顶部菜单【...】，点击【弹出储藏】
- 【命令面板】也支持弹出储藏，打开命令面板，输入`stash`或`pop`

## 弹出储藏、弹出最新储藏的区别

* 【弹出最新储藏】，恢复最近的一次进度
* 【弹出储藏】，会显示所有储藏列表。

<img src="/static/stash_pop.png" style="border: 1px solid #eee; margin: 20px 0;"/>

## Git 命令知识点：弹出储藏

```bash
$ git stash pop        
$ git stash pop stash@{0}       // 等于git stash pop，恢复最近的一次进度
$ git stash pop stash@{num}
```