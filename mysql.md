### 创建用户 授予权限

```
mysql -u root -h 127.0.0.1  -P 3307 -p

create user 'a'@'%' identified by ''******';';
grant all privileges ON a to  'a'@'%'; 

grant all privileges on *.* to 'root'@'%' identified by '*****';

revoke all privileges on a.* from  'xhfy'@'127.0.0.1'; #去除权限

drop user a@'127.0.0.1';

create user 'a'@'127.0.0.1' identified by '******';
grant all privileges ON a.* to  'a'@'127.0.0.1'; 

CREATE DATABASE battery DEFAULT CHARSET utf8 COLLATE utf8_general_ci;
```

https://zhuanlan.zhihu.com/p/612059265