
# 中文乱码问题

您在使用插件、或在终端使用git命令时，中文显示乱码，如下图：

<img src="/static/quote.png" style="border: 1px solid #eee;" />

## 解决方法

点击菜单【工具】【Git 命令面板】，输入`中文`

<img src="/static/quote_chinese.png" style="border: 1px solid #eee;"/>


## Git 命令

```
$ git config --global core.quotepath false
$ git config --global i18n.logoutputencoding utf-8      // 解决git log中文编码问题
```