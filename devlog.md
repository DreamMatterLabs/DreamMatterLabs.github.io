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

    <div class="row align-items-center m-0">
        {% for post in site.posts %}
          <a href="{{ post.url }}">
            <article class=" rounded post-preview fs-4" style="padding: 50px">
              <h2 class="fw-bold mb-3">{{ post.title }}</h2>
              <p class="text=white fw-normal m-0">{{ post.date | date: "%B %d, %Y" }}</p>
              <p class="text=white fw-normal m-0">{{ post.excerpt }}</p>
            </article>
          </a>       
        {% endfor %}
      </div>
  </div>

  <style>
    .post-preview 
    {
        background-color: #423B7A;
        box-shadow: 0px 0px 15px 5px rgba(0, 0, 0, 0.25);
        transition: box-shadow 0.3s ease-in-out;
    }

    .post-preview:hover 
    {
        box-shadow: 0px 0px 30px 5px rgba(80, 235, 236, 0.50);
    }
  </style>
</section>