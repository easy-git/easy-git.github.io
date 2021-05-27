# SSH Windows设置

> 本文仅适用于windows.

使用SSH克隆存储库之前，应确认已检查以下步骤：

- 您本地已生成SSH密钥，如果未生成，请先生成SSH密钥。[生成教程](/auth/ssh-generate)
- 已将SSH密钥添加到您的Git帐户。[设置教程](/auth/ssh-generate#Git服务器设置SSH公钥)
- 已启动SSH-Agent（适用于Windows用户，MacOSX用户不需要考虑）[教程](/auth/ssh-windows-set)
- 已将密钥添加到SSH代理（适用于Windows用户，MacOSX用户不需要考虑）[教程](/auth/ssh-windows-set)

## 启动SSH-Agent，并添加到SSH代理

> 本章节仅适用于windows。

1. 首先，打开`Git Bash`，注意名称，不是cmd也不是powershell
2. 启动ssh-agent
```
eval “$(ssh-agent -s)”
```
3. 添加SSH代码，即执行ssh-add
```
# id_rsa是证书文件名称，这里以id_rsa举例
ssh-add ~/.ssh/id_rsa
```

## 知识点

上面的文章，频繁的提到一个词 `SSH-Agent`, 那么什么是SSH-Agent？

ssh-Agent ，意为 ssh 代理，是一个密钥管理器，用来管理一个多个密钥，并为其他需要使用 ssh key 的程序提供代理。

SSH是一个允许两台电脑之间通过安全的连接进行数据交换的 网络协议。通过加密保证了数据的保密性和完整性。SSH采用 公钥 加密技术来验证远程主机，以及 (必要时) 允许远程主机验证用户。

而为了让其他程序更方便的使用这套加密技术，就有了 ssh agent。

当把私钥交给 ssh agent 管理的好处：

- 当 其他程序 需要身份验证的时候 可以将验证申请交给 ssh-agent 来完成整个认证过程。使用不同的密钥连接到不同的主机时，需要要手动指定对应的密钥，而ssh代理可以自动帮助我们选择对应的密钥进行认证。
- 避免重复输入密码：如果您的私钥使用密码短语来加密了的话，每一次使用 SSH 密钥对进行登录的时候，您都必须输入正确的密码短语。而 SSH agent 程序能够将您的已解密的私钥缓存起来，在需要的时候提供给您的 SSH 客户端。这样子，您就只需要在使用 ssh-add 时将私钥加入 SSH agent 缓存的时候，输入一次密码短语就可以了。这为经常使用 SSH 连接用户提供了不少便利。