# apple_dns
A simple DNS server. :-)

use 
python apple_dns.py 
to run this server. Then you can add domain and content in db.csv. Need no type.

Then you can dig/nslookup some domain in db.csv.


bug!!!!!!!!!

# test
```text
type可以是以下这些类型：

A 地址记录（直接查询默认类型）

AAAA 地址记录

AFSDB Andrew文件系统数据库服务器记录

ATMA ATM地址记录

CNAME 别名记录

HINFO 硬件配置记录，包括CPU、操作系统信息

ISDN 域名对应的ISDN号码

MB 存放指定邮箱的服务器

MG 邮件组记录

MINFO 邮件组和邮箱的信息记录

MR 改名的邮箱记录

MX 邮件服务器记录

NS 名字服务器记录

PTR 反向记录

RP 负责人记录

RT 路由穿透记录

SRV TCP服务器信息记录

TXT 域名对应的文本信息

X25 域名对应的X.25地址记录
```

- dig 
dig @dnsserver name querytype
dig @127.0.0.1 -p 9953 apple.tree


dig +tcp  @127.0.0.1  www.baidu.com A
dig +trace www.baidu.com

- nslookup
nslookup -port=9953 apple.tree 127.0.0.1