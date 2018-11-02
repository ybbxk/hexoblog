title: 便签
date: 2015-09-16 14:05:10
---
1.增加数据库用户权限  
```grant all privileges on dbname.* to username@'%' identified by 'password';```  
2.清除 DNS 缓存:  
chrome://net-internals/#dns  
3.[PHP程序员进阶学习书籍参考指南](http://blog.csdn.net/heiyeshuwu/article/details/50686878)  
4.git clone 后恢复文件修改时间:
```bash
git log --pretty=%at --name-status --reverse | perl -ane '($x,$f)=@F;next if !$x;$t=$x,next if !defined($f)||$s{$f};$s{$f}=utime($t,$t,$f),next if $x=~/[AM]/;'
```

