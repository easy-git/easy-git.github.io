---
date: 2021-01-15 22:19:35
---

# 查看储藏

- 在命令面板，输入`stash show`, 可以查看已储藏列表
- 选择储藏ID`stash{num}`, 可以查看`文件列表`、以及`内容差异`


<img src="/static/stash_show.gif" style="border: 1px solid #eee; margin: 20px 0;" />


## Git 命令知识点：查看储藏

```bash
$ git stash list
$ git stash show stash{num}         // 查看储藏中的文件列表
$ git stash show stash{num} -p      // 查看储藏中的文件内容差异
```