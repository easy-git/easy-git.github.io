---
date: 2021-01-09 22:19:35
---

# 如何获取 Git 项目仓库？

1. 在现存的目录下，通过导入所有文件来创建新的 Git 仓库。
2. 从已有的 Git 仓库克隆出一个新的镜像仓库来。

Git支持多种数据传输协议，通常有 `git://` 、`http(s)://`。

## 克隆

```
# 通过HTTPS协议克隆
git clone https://gitee.com/zxzllyj/sample-project.git

# 通过SSH协议克隆
git clone git@gitee.com:zxzllyj/sample-project.git
```

注意：使用SSH克隆，需要配置好SSH公钥。[配置SSH](/auth/ssh-generate)


## easy-git 克隆说明

- 支持`手动输入存储库url`，进行克隆。[查看详情](/connecting/clone)
- 如果当前设备，已通过[github、gitee认证](/oauth)，git url输入框，会`自动加载`github、gitee账号下所有的存储库地址；并已下拉列表形式展示存储库列表。
- 支持输入关键字，在github搜索存储库 [查看详情](/connecting/github-search)