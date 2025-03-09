---
layout: default
title: "Devlog & Updates"
permalink: /devlog/
---

<section class="devlog-container">
  <h1>Latest Devlog & Updates</h1>

  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-preview">
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.date | date: "%B %d, %Y" }}</p>
        <p>{{ post.excerpt }}</p>
      </article>
    {% endfor %}
  </div>
</section>