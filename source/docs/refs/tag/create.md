---
date: 2021-01-11 08:19:35
---

# 标签创建

创建标签的途径，通常有：

- 从当前分支上创建标签
- 指定commit_id创建标签

## 分支视图：从当前分支上创建标签

进入分支视图，选中当前分支，点击`标签`图标。如截图

<img src="/static/tag_create_01.png" style="border: 1px solid #eee; margin: 20px 0;" />

## 命令面板: 创建标签

<img src="/static/tag_create_02.png" style="border: 1px solid #eee; margin: 20px 0;" />

## Git 命令: 创建标签

```bash
$ git tag -a <tag_name> -m "message"
```

备注：`message`不是必须的，但是建议加上。