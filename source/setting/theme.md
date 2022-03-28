---
date: 2022-03-28 22:19:35
---

# 自定义主题

EasyGit, 已经适配HBuilderX 绿柔、酷黑、雅蓝主题。

同时，支持[HBuilderX 自定义主题](https://hx.dcloud.net.cn/Tutorial/themes?id=custom-window)，详细请参考HBuilderX自定义主题文档。

除此之外，EasyGit 1.7.4版本，设置项 `EasyGit.theme.siderBar`和`EasyGit.theme.editor` 用于自定义EasyGit源代码管理器视图和日志视图主题。

- 将以下json内容，拷贝到HBuilderX 【设置 - 源码视图】，注意内容格式。
- HBuilderX【设置 - 源码视图】，修改`EasyGit.theme.siderBar`和`EasyGit.theme.editor`值后，需要重启HBuilderX才能生效
- 自定义颜色，必须为十六进制颜色，比如`#FFFFFF`或`#FFF`


```json
// EasyGit 源代码管理器视图可自定义的颜色
"EasyGit.theme.siderBar": {
	"background": "",
	"fontColor": "",
	"lineColor": "",
	"inputColor": "",
	"inputBgColor": "",
	"inputLineColor": "",
	"scrollbarColor": "",
	"remarkTextColor": "",
	"menuBackground": "",
	"liHoverBackground": "",
	"cursorColor": ""
}
```


```json
// EasyGit 日志视图可自定义的颜色
"EasyGit.theme.editor": {
	"background": "",
	"fontColor": "",
	"lineColor": "",
	"inputColor": "",
	"inputBgColor": "",
	"inputLineColor": "",
	"scrollbarColor": "",
	"remarkTextColor": "",
	"menuBackground": "",
	"liHoverBackground": "",
	"cursorColor": ""
}
```

