---
layout: default
title: Content
---

{% for cate in site.categories %}
<h3>{{cate[0]}}</h3>
<ul>
    {% for post in cate[1] %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}