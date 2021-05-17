
---
date: 2021-01-09 22:19:35
---

# 生成新的 SSH 密钥并配置Git服务器

## 生成新SSH密钥

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

## SSH 密钥到 Git服务器

- [GitHub 帐户 添加SSH 密钥](https://docs.github.com/cn/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)
- [Gitee 码云设置SSH公钥](https://gitee.com/help/articles/4191)


