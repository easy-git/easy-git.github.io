---
date: 2021-01-09 22:19:35
---

# git clone - 克隆

1. HBuilderX 安装好EasyGit插件后，点击菜单【工具】【Git:克隆仓库】，即可打开视图界面。
2. 输入`仓库地址`，点击【开始克隆】按钮。
3. 注意：私有仓库，需要提供身份认证信息(比如`密码`或`SSH公钥`)，才能克隆。

<img src="/static/clone.gif" style="zoom: 50%; border: 1px solid #eee;" />

点击【开始克隆】，日志如下：

```
[Git] 12:33:02.880 开始克隆 testgit'！

[Git] 12:33:02.901 备注1：克隆进度跟项目大小、网络有关，需要一定时间，请不要重复点击【克隆】按钮。
[Git] 12:33:02.917 备注2：克隆成功后，会自动将克隆项目，加入到HBuilderX项目管理器。如未显示在项目管理器，请手动导入或拖入。

[Git] 12:33:02.932 Cloning into '/opt/test/testgit'...

[Git] 12:33:05.350 POST git-upload-pack (gzip 15631 to 7797 bytes)

[Git] 12:33:06.466 remote: Enumerating objects: 56562, done.        

[Git] 12:33:06.645 Git clone进度: 0%
[Git] 12:33:06.654 Git clone进度: 20%
[Git] 12:33:09.368 Git clone进度: 25%
[Git] 12:33:12.947 Git clone进度: 37%
[Git] 12:33:15.549 Git clone进度: 90%
[Git] 12:33:15.682 Git clone进度: 99%
[Git] 12:33:15.695 Git clone进度: 100%
[Git] 12:33:15.707 Git clone完成！
[Git] 12:33:15.723 Resolving deltas: 100% (39695/39695), done.

[Git] 12:33:16.940 克隆成功。本地路径: /opt/test/testgit
```