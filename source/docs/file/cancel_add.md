---
date: 2021-01-16 22:19:35
---

# 取消暂存的文件

如何操作`暂存区`和`工作目录中`已修改的文件？

例如，你已经修改了两个文件并且想要将它们作为两次独立的修改提交， 但是却意外地输入暂存了它们两个。如何只取消暂存两个中的一个呢？

源代码管理器视图，在【已暂存文件】列表，选中文件，点击`-`号，即可`取消暂存`。

<img src="/static/cancel_add.png" style="margin-bottom: 30px;"/>

## 取消所有暂存

<img src="/static/cancel_all_add.png" style="margin: 30px 0px;"/>


## Git 命令：取消暂存

```bash
$ git restore --staged <file>
$ git restore --staged *            // 取消所有暂存
```