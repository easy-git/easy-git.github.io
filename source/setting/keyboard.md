---
date: 2021-01-09 22:19:35
---

# 设置快捷键

easy-git, 支持通过快捷键打开git视图。

点击菜单【工具】【自定义快捷键】，可自定义快捷键。

##### 说明

- 目前只暴露了以下command。
- 请逐条拷贝，设置快捷键时，请仔细检查语法格式。
- 如需要更多commmand，请到[HBuilderX插件市场](https://ext.dcloud.net.cn/plugin?id=2475)留言。

```json
// 命令面板
{"key":"","command": "EasyGit.CommandPanel"}

// 打开Git文件视图
{"key":"","command": "EasyGit.main"}
 
// 查看日志
{"key": "","command": "EasyGit.log"}

// Git commit
{"key": "","command": "EasyGit.commit"}

// Git 修改最后提交的commit消息
{"key": "","command": "EasyGit.commitAmend"}

// Git克隆
{"key": "","command": "EasyGit.clone"}

// Git 文件对比
{"key": "","command": "EasyGit.diffFile"}

// Git restore 取消更改
{"key": "","command": "EasyGit.restore"}

// Git restore staged 取消暂存
{"key": "","command": "EasyGit.restoreStaged"}

// Git 撤销上一次commit
{"key": "","command": "EasyGit.resetSoftLastCommit"}

// Git 重置代码到上次提交
{"key": "","command": "EasyGit.resetHardLastCommit"}

// Git 重置代码到指定提交
{"key": "","command": "EasyGit.resetHardCommitID"}

// Git pull --rebase
{"key": "","command": "EasyGit.pull"}

// Git stash 储藏
{"key": "","command": "EasyGit.stash"}

// Git stash 储藏全部(包含未跟踪的)
{"key": "","command": "EasyGit.stashAll"}

// Git stash 弹出储藏
{"key": "","command": "EasyGit.stashPop"}

// Git stash 弹出最新储藏
{"key": "","command": "EasyGit.stashPopNew"}

// Git stash 删除所有储藏
{"key": "","command": "EasyGit.stashClear"}

// Git stash 查看某个储藏的文件列表以及差异
{"key": "","command": "EasyGit.stashShow"}

// Git Blame 显示git文件当前行最后一次修改信息
{"key": "","command": "EasyGit.gitBlameForLineChange"}

// Git tag 创建标签
{"key": "","command": "EasyGit.tagCreate"}

// Git tag 查看标签详情
{"key": "","command": "EasyGit.tagDetails"}

// Git init
{"key": "","command": "EasyGit.init"}

// Git add Remote Origin
{"key": "","command": "EasyGit.addRemoteOrigin"}

// Git merge
{"key": "","command": "EasyGit.merge"}

// Git merge --abort
{"key": "","command": "EasyGit.mergeAbort"}

// Git Branch switch
{"key": "","command": "EasyGit.BranchSwitch"}

// Git Branch Delete
{"key": "","command": "EasyGit.BranchDelete"}

// Git Branch Diff
{"key": "", "command": "EasyGit.BranchDiff"}

// Git Branch diff file 显示两个分支指定文件的差异
{"key": "", "command": "EasyGit.twoBranchSpecificFileDiff"}

// Git reflog
{"key": "","command": "EasyGit.reflog"}

// Git 归档
{"key": "","command": "EasyGit.archive"}

// Git 查看文件在另一个分支的内容(无需切换分支)
{"key": "","command": "EasyGit.showAnotherBranchFile"}

// Git 在浏览器查看Git仓库
{"key": "","command": "EasyGit.openGitRepositoryInBrowser"}

// Git cofing --list
{"key": "","command": "EasyGit.showConfig"}

// Git oauth
{"key": "","command": "EasyGit.oauth"}

// Git 创建远程仓库
{"key": "","command": "EasyGit.CreateRemoteRepository"}

// 删除远程仓库url
{"key": "","command": "EasyGit.RemoteRmOrigin"}

// Git 查看文件的历史提交版本内容
{"key": "","command": "EasyGit.showHashFile"}
```