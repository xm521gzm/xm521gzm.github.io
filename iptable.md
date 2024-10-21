## How to understand CIDR
```
172.17.0.111/20
top 20 change 1 is network part 网络部分
bottom 12 change 0 is host part 主机部分
```

### network part: 

```
11111111 11111111 11110000 00000000
255.255.240.0
```
### network address: 网络地址
```
172.17.0.111 "AND" with 255.255.240.0

B = 10101100 00010001 00000000 11011110
A = 11111111 11111111 11110000 00000000
C = B "AND" A = 10101100 00010001 00000000 00000000
C = 172.17.0.0
```

### broadcast address: 广播地址 = 网络地址后12位变1
```
network address bottom 12 change 1 
10101100 00010001 00001111 11111111
D = 172.17.15.255
```
### finally: 
```
172.17.0.1 ~ 172.17.15.254
172.17.0.0 network address
172.17.15.255 broadcast address

```

```shell
iptables -I INPUT -s 117.133.17.237 -p tcp -m multiport --dports 80,443 -j DROP
```

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


