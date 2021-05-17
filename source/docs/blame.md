---
date: 2021-01-15 22:19:35
---

# git blame: 显示当前行最后一次修改信息

如下图所示：

1. 编辑器，打开要查看的文件，将`光标`置于要查看的`行`
2. 右键菜单，点击【显示当前行最后一次修改信息】
3. 结果会出现`底部状态栏`

<img src="/static/blame.png" style="border: 1px solid #eee;" />

Git 命令扩展：

```bash
$ git blame -L 2,2 <filename>
```