---
date: 2021-01-16 22:19:35
---

# 撤销修改

如何从工作区撤销文件修改？

源代码管理器视图，【更改】列表


<img src="/static/cancel_change.png" style="margin-bottom: 30px;"/>


## Git 命令：撤销修改


```bash
$ git restore <file>         // 撤销指定文件
$ git restore <dirname>/     // 撤销指定目录下，所有文件修改
$ git restore：/             // 撤销工作区所有文件修改
$ git restore .              // 撤销当前目录所有修改
$ git restore *              // 撤销当前目录所有修改
$ git restore *.js           // 撤销指定后缀的文件，比如js

$ git checkout -- <file>
```

备注：`git checkout`和`git restore`都可以实现从工作区撤销修改的功能。但是，不推荐使用`git checkout`

## git restore的来源

`git checkout`命令承载了分支操作和文件恢复的部分功能，有点复杂，并且难以使用和学习。

所以Git社区将这两部分功能拆分开，在git `2.23.0`中引入了两个新的命令`restore`和`switch`


