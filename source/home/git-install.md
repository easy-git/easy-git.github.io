# Git工具

> 如果您的电脑已安装Git命令行工具，请跳过本章。

easy-git插件，本质是调用的git命令，请确保电脑已安装git工具。


## Windows

Windows需要电脑本机安装git-bash，[Git Bash下载地址](https://git-scm.com/download/win)


> 如果上面的地址，无法访问，请用迅雷直接使用下面的地址进行下载：

windows git安装包，是一个exe文件，双击打开，不停的【下一步】即可完成安装。

[windown 32bit git下载地址](https://github.com/git-for-windows/git/releases/download/v2.31.1.windows.1/Git-2.31.1-32-bit.exe)
[windows 64bit git下载地址](https://github.com/git-for-windows/git/releases/download/v2.31.1.windows.1/Git-2.31.1-64-bit.exe)


## MacOSX

> MacOSX 部分机型自带git工具，如果没有，可以通过[brew](https://brew.sh/index_zh-cn)安装git命令工具

安装命令：
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install git
```

如果brew因网络问题安装失败，请参考：[详情](https://www.jianshu.com/p/06a9a59e7040)

## 问题排查

> 再次说明，easy-git插件，本质是调用的git命令，请确保电脑已安装git工具。

打开`操作系统终端命令行`软件，输入`git --version`, 检查下命令是否存在。

如果终端出现下列错误，则说明git`没有`安装成功。

- 错误1： `'git' 不是内部或外部命令，也不是可运行的程序或批处理文件。`
- 错误2：`git: command not found`

> 特别注意：windows电脑，如果您确定已成功安装Git安装包，但是命令行还是出现上面的错误，请将git安装目录加入到系统环境变量。

如果您还无法解决问题，请加入QQ交流群寻求帮助: 623513298 [点击加入](https://qm.qq.com/cgi-bin/qm/qr?k=QRbb77rmIhpsh8OthaftVWfYZQdBr_Ir&jump_from=webapi)