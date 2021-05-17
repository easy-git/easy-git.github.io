# OAuth授权认证

授权easy-git获取Github、gitee等`git托管服务器`访问凭证后，您可以在HBuilderX内，通过easy-git使用远程Git服务器某些功能，比如创建远程仓库、读取远程仓库列表，而无需再登录浏览器，操作更便捷。

比如：克隆操作，之前您首先需要拷贝仓库地址，拷贝的操作（打开浏览器、打开github、找到仓库、拷贝url），授权后，您就可以省略这些步骤。

授权后`访问凭证`仅会存储在您的个人电脑上，`不会上传网络`，也不会在网络上保存您的任何信息，它们仅保存在您的个人电脑上，且已`加密`。

## 1. 目前支持的功能

- 插件内，创建远程仓库（支持github、gitee) [查看详情](/extensions/create-remote-repo)
- 插件内，搜索Github并克隆 [查看详情](/connecting/github-search)

## 2. 打开授权

顶部菜单【工具 - easygit - OAuth授权】，或命令面板中搜索`oauth`都可以打开授权窗口。

如下附件所示，目前仅支持github和gitee，后期会增加对内部使用gitlab搭建git托管服务器的支持，请等待。

点击弹窗中的【gitee】或【github】,即可跳转到相关网页进行授权。

<img src="/static/oauth.min.png" style="zoom: 50%; border: 1px solid #eee; border-radius: 20px;"/>

#### 2.1 Gitee授权认证

如下图所示，当您点击【gitee】后，将会跳转到浏览器并打开如下页面

`【查看、创建、更新你的项目】`，勾选权限后，您可以在HBuilderX内 查看、创建远程仓库，而无需再打开浏览器进行创建。

<img src="/static/oauth-gitee.png" style="zoom: 45%; border-radius: 5px;"/>