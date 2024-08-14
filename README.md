# QFNU-JWC-Tracker

曲阜师范大学教务处公告监控

每 5 分钟检查一次教务处公告，有新公告时提取标题，摘要，链接，推送至群聊

qfnujwc-on 开启教务处公告监控

qfnujwc-off 关闭教务处公告监控

qfnuzcc-on 开启资产处公告监控

qfnuzcc-off 关闭资产处公告监控

## 更新日志

2024 年 8 月 13 日，优化逻辑，由原来的定时任务改为通过每五秒心跳检测调用函数，减少任务创建的内存占用。

2024 年 8 月 14 日，修复开关失效的 bug（实际上是忘了写调用）

2024 年 8 月 14 日，优化逻辑，由原来的每个群聊单独创建一个任务改为所有群聊共用一个任务，减少内存占用

2024 年 8 月 14 日，增加网页内容获取失败的处理逻辑，防止因为网络问题导致脚本崩溃

2024 年 8 月 14 日，新增曲阜师范大学资产处公告监控

2024 年 8 月 14 日，修复由于只有一个上次监控时间，导致每次执行时都会只执行一次的 bug
