数据库类型

> 数值类型

+  整数类型
	+ TINYINT(很小的整数) SMALLINT(小的整数) MEDIUMINT(中等大小的整数) INT(普通大小的整数) BIGINT(大整数)
+  浮点小数数据类型
	+ FLOAT DOUBLE 定点小数类型DECIMAL
+ 日期类型
	+ YEAR TIME DATE DATETIME TIMESTAMP
	+ TIME 用于只是需要时间信息的值 格式为 HH:MM:SS
	+ 时间格式解释
		+ D HH:MM:SS 天 小时 分钟 秒
		+ 10:07:09 -> 10:07:09
		+ 23:23 -> 23:23:00
		+ 2 10:10 58:10:0
		+ 3 02 -> 74:00:00
		+ 10 -> 00:00:10

+ 字符串类型
	+ CHAR VARCHAR BINARY VARBINARY BLOB TEXTENUM SET
	+ 字符串类型分为文本字符串和二进制字符串

> 删除表中的数据

delete from tb1;