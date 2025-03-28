---
layout: default
title: "Devlog & Updates"
permalink: /devlog/
body_class: blog-page
---

<section class="devlog-container">
  <div class="section-header text-center">
    <h1 class="m-0 fs-4 text-uppercase text-muted2">Devlog & Updates</h1>
  </div>

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