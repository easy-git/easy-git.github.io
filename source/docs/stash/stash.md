---
date: 2021-01-15 22:19:35
---

# git stash: 储藏

> git stash, 它是 Git 最有用的功能之一

## 好处

- stash会把所有未提交的修改（包括暂存的和非暂存的）都保存起来，用于后续恢复当前工作目录。
- 储藏后，会将当前代码切换到`HEAD`提交上.
- 储藏后，回到之前最后一次提交的干净的工作仓库。

## 应用举例

- 做了一半的需求, 需要先做别的需求
- 开发一半功能, 需要同步远端代码。如果冲突呢？遇到这种情况, 可以先保存本地修改, 进行`git pull`, 然后再`pop`出本地代码。
- 提交特定文件。如果对多个文件做了修改,但是只想提交几个文件, 或者想先暂时保存几个修改,测试其他文件的执行结果.可以通过`git stash save --keep-index`来进行.

## 如何使用？

- easy-git源代码管理器视图，点击顶部菜单【...】，点击【储藏】，然后输入`储藏消息`
- 打开命令面板，搜索`stash - 储藏`, 弹框，然后输入`储藏消息`

<div style="margin: 1rem 0 1rem 1rem;">
    <img src="/static/stash.png" />
</div>

## 储藏、储藏全部的区别

默认情况下，git stash会缓存下列文件：

- 添加到暂存区的修改（staged changes）
- Git跟踪的但并未添加到暂存区的修改（unstaged changes）

但不会缓存以下文件：

- 工作目录中，新建的文件（untracked files）
- 被忽略的文件（ignored files）

储藏全部，会储藏当前目录下的所有修改

## Git 命令知识点：储藏

```bash
$ git stash
$ git stash save "message"  // 建议给每个stash加一个message，用于记录版本
$ git stash -a              // stash当前目录下的所有修改
$ git stash -u              // stash untracked文件
```