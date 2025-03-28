---
layout: default
title: "Devlog & Updates"
permalink: /devlog/
body_class: blog-page
---

<section class="devlog-container">
  <div class="container d-flex flex-column" style="padding-top: 50px; padding-bottom: 150px; row-gap: 100px">
    <div class="section-header text-center">
      <h1 class="m-0 fs-4 text-uppercase text-muted2">Devlog & Updates</h1>
    </div>

    <div class="rounded blogpost">
      <div class="row align-items-center p-5 m-0">
        {% for post in site.posts %}
          <article class="post-preview text=white fs-4">
            <h2 class="fs-4 fw-bold mb-3" ><a href="{{ post.url }}">{{ post.title }}</a></h2>
            <p class="fw-normal m-0">{{ post.date | date: "%B %d, %Y" }}</p>
            <p class="fw-normal m-0">{{ post.excerpt }}</p>
          </article>
        {% endfor %}
      </div>
    </div>
  </div>

  <style>
    .post-preview 
    {
        background-color: #423B7A
        box-shadow: 0px 0px 15px 5px rgba(0, 0, 0, 0.25);
        transition: box-shadow 0.3s ease-in-out;
    }

    .post-preview:hover 
    {
        box-shadow: 0px 0px 30px 5px rgba(80, 235, 236, 0.50);
    }
  </style>
</section>