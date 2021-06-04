
---
date: 2021-01-09 22:19:35
---

# SSH Key生成，并配置Git服务器

* [一键自动生成SSH密钥](#一键自动生成SSH密钥)
* [手动生成SSH密钥](#手动生成SSH密钥)

## 一键自动生成SSH密钥

> easy-git插件，1.4.6版本，新增了SSH密钥一键自动生成功能。
> 如果easy-git版本，低于1.4.6，请手动打开`操作系统终端`手动生成。

安装easy-git插件到HBuilderX后，点击菜单【工具】【easy-git】【一键生成SSH KEY】; 或打开命令面板，搜索SSH

1. SSH Key生成工具，调用的是ssh-keygen命令，支持四种算法，如果不确定使用哪种，默认即可。
2. 生成的ssh key存储在`~/.ssh/`目录下。
3. SSH Key用途默认不勾选，如果您是用于Git服务器，强烈建议勾选，并提供Git域名，以方便添加到`~/.ssh/config`中。如果您不了解`~/.ssh/config`，请自行搜索相关知识，这是一个很有用的配置。
4. 生成成功后，会自动执行ssh-add将新生成的密钥添加到ssh-agent中。

<img src="/static/ssh-keygen.png" style="zoom: 90%;border: 1px solid #eee;" />

## 手动生成SSH密钥

1. 打开 Terminal（终端）或Git Bash。
2. 粘贴下面的文本（替换为您的 GitHub 电子邮件地址）。

```bash
$ ssh-keygen -t ed25519 -C "your_email@example.com"
```

注：如果您使用的是不支持 Ed25519 算法的旧系统，请使用以下命令：
```bash
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

3. 提示您“Enter a file in which to save the key（输入要保存密钥的文件）”时，按 Enter 键。 这将接受默认文件位置。

```bash
> Enter a file in which to save the key (/Users/you/.ssh/id_ed25519): [Press enter]
```

4. 添加到ssh代理

```bash
# filepath为您刚才生成的SSH证书路径。
ssh-add ~/.ssh/<filepath>
```

## Git服务器设置SSH公钥

- [GitHub 帐户 添加SSH 密钥](https://docs.github.com/cn/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)
- [Gitee 码云设置SSH公钥](https://gitee.com/help/articles/4191)


