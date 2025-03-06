---
layout: post
title: "Devlog & Updates"
permalink: /devlog/
---
<ul>
{% for post in site.posts %}
 <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>