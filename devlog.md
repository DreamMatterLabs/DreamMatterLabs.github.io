---
layout: default
title: "Devlog & Updates"
permalink: /devlog/
---

<h1>Latest Updates</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>