
---
date: 2021-01-09 22:19:35
---

## 检查现有 SSH 密钥

在生成 SSH 密钥之前，您可以检查是否有任何现有的 SSH 密钥。

1. 打开 Terminal（终端）Terminal（终端）Git Bash。
2. 输入 `ls -al ~/.ssh` 以查看是否存在现有 SSH 密钥：

```bash
$ ls -al ~/.ssh
```

3. 检查目录列表以查看是否已经有 SSH 公钥。 默认情况下，公钥的文件名是以下之一：

```bash
id_rsa.pub
id_ecdsa.pub
id_ed25519.pub
```

如果您没有现有的公钥和私钥对，或者不想使用任何可用于连接到 GitHub 的密钥对，则生成新的 SSH 密钥。
