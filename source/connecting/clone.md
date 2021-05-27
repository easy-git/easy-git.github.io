---
date: 2021-01-09 22:19:35
---

# git clone - 克隆

1. HBuilderX 安装好EasyGit插件后，点击菜单【工具】【Git:克隆仓库】，即可打开视图界面。
2. 输入`仓库地址`，点击【开始克隆】按钮。
3. https方式克隆，如果是私有仓库，需要提供身份认证信息(比如`密码`)，才能克隆。
4. SSH方法克隆，请参考本文第二章节。

<img src="/static/clone.gif" style="zoom: 50%; border: 1px solid #eee;" />

点击【开始克隆】，日志如下：

```
[Git] 12:33:02.880 开始克隆 testgit'！

[Git] 12:33:02.901 备注1：克隆进度跟项目大小、网络有关，需要一定时间，请不要重复点击【克隆】按钮。
[Git] 12:33:02.917 备注2：克隆成功后，会自动将克隆项目，加入到HBuilderX项目管理器。如未显示在项目管理器，请手动导入或拖入。

[Git] 12:33:02.932 Cloning into '/opt/test/testgit'...     

[Git] 12:33:06.645 Git clone进度: 0%
[Git] 12:33:06.654 Git clone进度: 20%
[Git] 12:33:15.682 Git clone进度: 99%
[Git] 12:33:15.695 Git clone进度: 100%
[Git] 12:33:15.707 Git clone完成！
[Git] 12:33:15.723 Resolving deltas: 100% (39695/39695), done.

[Git] 12:33:16.940 克隆成功。本地路径: /opt/test/testgit
```

# ssh_clone

使用SSH克隆存储库之前，应确认已检查以下步骤：

- 您本地已生成SSH密钥，如果未生成，请先生成SSH密钥。[生成教程](/auth/ssh-generate)
- 已将SSH密钥添加到您的Git帐户。[设置教程](/auth/ssh-generate#Git服务器设置SSH公钥)
- 已启动SSH-Agent（适用于Windows用户；MacOSX用户不需要考虑）[教程](/auth/ssh-windows-set)
- 已将密钥添加到SSH代理（适用于Windows用户；MacOSX用户不需要考虑）[教程](/auth/ssh-windows-set)


> MacOSX默认包含SSH-Agent，如果您是通过[SSH一键生成工具](/auth/ssh-generate)生成的密钥，则无需任何额外的工作；否则您需要手动运行ssh-add添加SSH密钥，只需要执行一次。
> 
> Windows需要则需要额外执行一些步骤，[参考](/auth/ssh-windows-set)

特别注意：

1. 如果上述操作进行后，SSH克隆仍失败，请在操作系统终端，自行运行克隆命令。
2. windows电脑，SSH克隆非常麻烦，使用easy-git克隆失败的可能性非常大，请启动`Git Bash`进行克隆。

克隆命令：

```
git clone <url>
```

# 克隆错误

### 错误1: Permission denied (publickey)

原因：本地没有 SSH Key文件，或本地的ssh key跟远程git服务器ssh信息不匹配。

解决方法：

1. 如果本地没有配置ssh key，请生成SSH密钥，并添加SSH公钥到远程服务器。[SSH key生成教程](/auth/ssh-generate)
2. windows电脑，如果在easy-git内使用ssh无法克隆成功，请打开`Git Bash`手动克隆仓库。

### 错误2: Incorrect username or password

原因：如果您采用http的方式克隆，如果用户或密码错误，克隆时则会提示：Incorrect username or password

解决方法：输入正确的用户名或密码。