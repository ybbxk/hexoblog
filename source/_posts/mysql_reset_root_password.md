title: 重置mysql root密码
date: 2015-10-26 17:04:19
tags: [mysql]
---
新的项目要用mysql5.6.x，centos默认的yum库只有mariadb，兼容mysql5.5。
看msyql文档装了社区版的5.7，却无法进入mysql，看到网上介绍的mysqld_safe指令重置密码，却发现5.7没有mysqld_safe指令。郁闷ing，再没找到其它方法，只能卸载5.7，安装5.6。  

https://dev.mysql.com/doc/refman/5.0/en/resetting-permissions.html
