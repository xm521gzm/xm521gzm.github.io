/data/part1/logs/supervisor/log/bag* | grep  -E 'pinshi|2,1\&1'

$grep -10 ‘123’ test.log//打印匹配行的前后10行
或
$grep -C 10 ‘123’ test.log//打印匹配行的前后10行
或
$ grep -A 10 -B 10 ‘123’ test.log //打印匹配行的前后10行

$grep -A 10 ‘123’ test.log //打印匹配行的后10行

$grep -B 10 ‘123’ test.log//打印匹配行的前10行
————————————————
版权声明：本文为CSDN博主「小西blue」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/huashao0602/article/details/78018743

