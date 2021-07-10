---
date: 2021-01-09 22:19:35
---

# git fetch

git fetch 并没更改本地仓库的代码，只是拉取了远程 commit 等数据

当您打开Git源代码管理器时，easy-git插件会自动进行git fetch操作。

## 问题1

> could not read Username

[解决方法](/question/username)

## 问题2

> Permission denied (publickey).

出现此问题的原因，通常有：
- 远程Git服务器没有添加公钥
- 本地没有生成SSH公钥
- 没有配置`~/.ssh/config`
- 本地SSH秘钥没有加入到ssh-agent的高速缓存（如果没有特殊配置，每次重启电脑后都需要使用ssh-add重新添加）。如果已配置`~/.ssh/config`，请忽略。

~/.ssh/config配置文件格式（以github为例）:

```
Host github
	HostName github.com
	PreferredAuthentications publickey
	IdentityFile <ssh私钥文件绝对路径>
```