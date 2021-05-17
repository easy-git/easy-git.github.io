---
date: 2021-01-10 12:19:35
---

# git log 日志搜索

- 搜索, 支持`git log`所有参数
- 唯一不同的是多个参数之间，以`逗号`分隔。
- 当使用`--grep`、`--author`、`--after`等带有 `--` 的参数进行查询时，必须使用` = `，不支持`空格`


<img src="/static/log-search.png" style="border: 1px solid #eee; margin: 20px 0;" />

## 搜索条件示例

搜索作者`小明`、提交消息带有`新增`的5条日志。

推荐的搜索条件：

```
--author=小明,--grep=新增,-n 5
```

`错误`的搜索条件：

```
--author 小明,--grep 新增, -n 5
```

备注：此方法在命令行是可以正常使用的，受限于框架，此种搜索会导致错误。


## git log 参数

|搜索				|说明										|例子				|
|--					|--											|--					|
|--author			|按作者搜索									|--author='name'	|
|--after; --since	|搜索xx日期之后								|--after='2020-7-1'	|
|--before; --until	|搜索xx日期之前								|--before='2020-7-1'|
|-n					|仅显示最近的 n 条提交						| -n 10				|
|--grep				|用 --grep 选项搜索提交说明中的关键字		|--grep=xxxx		|
| 文件名称			|按文件查看log, 直接输入文件名即可			|					|
| -S				|仅显示添加或删除内容匹配指定字符串的提交	    | -S xxxx			|
|--committer		| 仅显示提交者匹配指定字符串的提交			|--committer=xxxx	|