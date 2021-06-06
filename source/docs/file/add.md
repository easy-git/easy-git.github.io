---
date: 2021-01-09 22:19:35
---

# git add 将文件添加到暂存区


如下图所示：

- 当本地有文件发生变动时，将会出现在【更改】列表中；暂存成功，将会出现在【暂存的更改】列表中。
- 在【更改】列表，选中文件，点击`+`号，即可将文件`加入`暂存区；
- 在【更改】列表，选中文件，点击`-`号，即可`撤销`文件修改。

<img src="/static/add.gif" />

Git 命令扩展：

```bash
$ git add <filename>           // 添加指定文件
$ git add <dirname>            // 添加指定目录（含子目录）
$ git add .                    // 添加当前目录下的所有文件到暂存区
$ git add *                    // 添加所有

$ git restore <file>           // 撤销修改
$ git restore --staged <file>  // 撤销暂存
```