title: 段落效果
date: 2015-10-10 13:56:30
categories: 前端
tags: [css,hexo,前端]
---
<style type="text/css">
p.d_s{text-indent: 2em;}
p.fd:first-letter:first-child {font-size:2.5em; font-family:"楷体","楷体_GB2312"; font-weight:bold; line-height:1.2em; float:left; padding:5px 2px 0 0; color:#c00;}
</style>
按照中文的习惯，每段都要空两个字符，结果用markdown时，发现手动输入的空格都被过滤了，无效。搜索一番后找到方法，两个`&emsp;`即可解决。  
<p class="d_s" style="text-indent: 2em;">但是每次都要手动输入，比较麻烦，想到了用css解决，加入这么一段就OK
`p{text-indent: 2em;}`</p>
<p class="f_d"><div style="font-size:2.5em; font-family:'楷体','楷体_GB2312'; font-weight:bold; line-height:1.2em; float:left; padding:5px 2px 0 0; color:#c00;">脑</div>洞大开，又想到了其它效果，**首字下沉**，也找到了相应的css  </p>
`p:first-letter:first-child {font-size:2.5em; font-family:"楷体","楷体_GB2312"; font-weight:bold; line-height:1.2em; float:left; padding:5px 2px 0 0; color:#c00;}`  
