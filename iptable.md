iptables -I INPUT -s 117.133.17.237 -p tcp -m multiport --dports 80,443 -j DROP

-P	设置默认策略
-F	清空规则链
-L	查看规则链
-A	在规则链的末尾加入新的规则
-I num	在规则链的头部加入新的规则
-D num	删除某一条规则链
-s	匹配来源的ip/MASK
-d	配置目标地址
-i 网卡名称	匹配这块网卡流入的数据
-o 网卡名称	匹配这块网卡流出的数据
-p	匹配协议，例如：TCP，UDP，ICMP
–dport num	匹配目标端口号
–sport num	匹配来源端口号
-j	指定匹配到数据包后的动作，如 ACCEPT、DROP、REJECT等。


