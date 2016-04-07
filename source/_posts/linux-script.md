title: linux脚本
date: 2016-04-07 17:04:20
tags: linux
---
1.使用cp时强制覆盖，两种方案:([来源](http://stackoverflow.com/a/8488293))
a) ` /bin/cp -rf /zzz/zzz/* /xxx/xxx `
b) ` /bin/cp -rf /zzz/zzz/* /xxx/xxx `  
原来当使用root登陆时，环境变量中会有一条 ` alias cp = cp -i ` ，用于防止管理员误操作。

2.tt
