# 要点记录

> 题目:第 0020 题： 登陆中国联通网上营业厅 后选择「自助服务」 --> 「详单查询」，然后选择你要查询的时间段，点击「查询」按钮，查询结果页面的最下方，点击「导出」，就会生成类似于 2014年10月01日～2014年10月31日通话详单.xls 文件。写代码，对每月通话时间做个统计。


## 记录

因为本人是移动卡，所以换成了移动的某个导出数据（为隐私excel 文件中删除了无关的信息）。

excel 文件中的通话时间都是`xx分xx秒`或`xx秒`的格式，十分固定。因此只需要判断不同情况统计分、统计秒，最后统一计算就可以了。当然，本代码的验证方式比较流氓，直接通过len 区分不同情况的。