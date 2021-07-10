# Permission denied (publickey)

### 错误

```
 Error: git@gitee.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

### 原因

出现此问题的原因，通常有：
- 远程Git服务器没有添加公钥
- 本地没有生成SSH公钥 [方法](/auth/ssh-generate)
- 没有配置`~/.ssh/config`
- 本地SSH秘钥没有加入到ssh-agent的高速缓存（如果没有特殊配置，每次重启电脑后都需要使用ssh-add重新添加）。如果已配置`~/.ssh/config`，请忽略。

~/.ssh/config配置文件格式（以github为例）:

```
Host github
	HostName github.com
	PreferredAuthentications publickey
	IdentityFile <ssh私钥文件绝对路径>
```