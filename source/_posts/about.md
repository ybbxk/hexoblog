title: about
date: 2015-09-15 12:18:39
tags:
---
试着用一次
{% for link in site.data.menu %}
<a href="{{ link }}">{{ loop.key }}</a>
{% endfor %}
