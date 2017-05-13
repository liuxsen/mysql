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
			+ current_time() now() 表示的是当前的时间

	+ DATE 用于只是需要日期值时，没有时间部分
		+ 日期格式为
		+ YYYY-MM-DD  (00-69) 转化为 20 (69-99) 转化为 19
		+ 输入 '2012-12-31' 、 '20121231' 都可以
		+ current_date() now()  表示的当前日期
	
	+ DATATIMER 用于同时需要日期和时间
		+ 格式为 YYYY-MM-DD HH:MM:SS   YYYYMMDDHHMMSS
		+ 可以使用字符串或者数值类型插入；只要符合格式就可以
		+ current_time() now() 表示的是当前的时间
		
	+ TIMESTAP
		+ 跟datetime 类似
	
+ 字符串类型
	+ CHAR VARCHAR BINARY VARBINARY BLOB TEXTENUM SET
	+ 字符串类型分为文本字符串和二进制字符串
	+ CHAR
		+ 为固定字符串 char(m) 0~255 char(4) 固定长度的字符串，字符长度最大为4；
		+ 会删除掉尾部的空格
	+ varchar 
		+ 长度可变的字符串，总是加一个字符串结束字符
		+ 所占的字节数为实际长度加1；


> 删除表中的数据

delete from tb1;