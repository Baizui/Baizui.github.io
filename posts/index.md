---
layout: archive
title:  "文章"
date: 2018-01-03 22:07:50 
modified:
excerpt: ""
tags: []
---
Web 分类（categories）
{% for post in site.categories.rwd %}- 
	<a href='{{ site.url }}{{ post.url }}'>{{ post.title }}</a>
{% endfor %}

信息可视化笔记 分类（categories）
{% for post in site.categories.infovis %}
	<a href='{{ site.url }}{{ post.url }}'>{{ post.title }}</a>
{% endfor %}