---
layout: page
title: 主页
tagline: hahaha
---
{% include JB/setup %}
主页怎么可以这么丑

## 这特么是我所有的文章啦！

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


