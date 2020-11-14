| Name                    |   归属   | 属性   | 说明                                                         |
| ----------------------- | :------: | ------ | ------------------------------------------------------------ |
| `XMLY_SPEED_COOKIE`     | 喜马拉雅 | 非必须 | [Cookie获取请参考](https://github.com/Zero-S1/xmly_speed/blob/master/xmly_speed.md),仅支持git actions执行,多个Cookie用换行即可 |
| `XMLY_ANDROID_AGENT`     | 喜马拉雅 | 非必须 | 仅安卓用的Agent配置，不填的话也会默认用红米8的 |
| `XMLY_ACCUMULATE_TIME`     | 喜马拉雅 | 非必须 | 需要刷时长任务的话，填入`zero_s1`；可能会黑号，请知悉 |
| `XMLY_ACCUMULATE_INDEX`     | 喜马拉雅 | 非必须 | 需配合`XMLY_ACCUMULATE_TIME`使用，用于限定某个索引的账号不进行刷时长 |
| `XMLY_ACCUMULATE_HOURS`     | 喜马拉雅 | 非必须 | 需配合`XMLY_ACCUMULATE_TIME`使用，用于限定每天收听的小时数,尽量避免黑号 |

##### 关于`XMLY_ACCUMULATE_INDEX`

> 用于指定哪几个账号不执行时长任务

比如我有5个账号，我第1个和第5个不想执行刷时长任务，则填入内容为`1,5`
例如我只有两个号，第2个号不想执行刷时长，则直接填入`2`即可

##### 关于`XMLY_ACCUMULATE_HOURS`

> 用于指定时长任务最大时间，防止现在时长任务直接是24小时的，过于容易发生黑号情况

传入`1`~`24`之间的数字即可