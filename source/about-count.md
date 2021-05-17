# 数据统计说明

与大多数应用一样，本插件也需要统计某些功能点的使用情况。

获取数据的目的，是为了决定是否强化或下线本软件的某些功能。

将来本插件趋于完善之后，将停止统计。

## 打点详细字段说明

统计数据包含，当天插件是否被人使用、电脑操作系统信息（字段内容windows、mac）。

如不希望上传操作系统信息, 请在【设置】【源码视图】内，增加如下字段:

```shell
"EasyGit.isShareUsageData": false
```