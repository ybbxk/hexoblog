title: PHP学习笔记
date: 2015-09-17 13:52:57
tags: [php,study,note]
---
1、销毁一个session变量使用`unset($_SESSION['myvar']_)`;
我们不能销毁整个`$_SESSION`数组(`unset($_SESSION`)),因为这样将禁用会话功能。要一次销毁所有的会话变量，可以使用如下所示语句：
```$_SESSION = array();```
当使用完一个会话后，首先应该注解所有的变量，然后再调用：`session_destroy();`来清除会话ID  
  
2、**eval()** 把字符串作为PHP代码执行  
 
3、`is_file()` 和 `file_exists()` 的区别：当参数是**目录**时，`file_exists()`返回 `true`，`is_file()` 返回`false`;
4、 `__autoload()`和`spl_autoload_register()`都是自动加载php文件。区别是：`spl_autoload_register()`高效且支持多个，方便在框架中和在第三方库时使用。`__autoload()`可能在后期的版本中弃用。所以尽量使用`spl_autoload_register()`。
