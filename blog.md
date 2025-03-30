---
layout: default
title: "Blog"
permalink: /blog/
body_class: blog-page
---
<section class="devlog-container">
  <div class="container d-flex flex-column" style="padding-top: 150px; padding-bottom: 150px; row-gap: 50px">
    <div class="section-header text-center">
      <h1 class="fw-bold text-uppercase text-white m-0" style="font-size: 2.45rem">Blog</h1>
    </div>

    <div class="row align-items-center" style="gap: 50px">
        {% for post in site.posts %}
          <a class="text-decoration-none text-white" href="{{ post.url }}">
            <article class="post-preview">
              <img class="img-fluid rounded post-banner" style="width: 100%; aspect-ratio: 16 / 9" src="{{ post.banner }}">

              <div class="col d-flex" style="flex-direction: column; padding: 50px">         
                <p class="fs-5 fw-normal m-0 p-0">{{ post.date | date: "%B %d, %Y" }}</p>   
                <h2 class="fs-1 fw-bold mb-3 p-0">{{ post.title }}</h2>                         
                <p class="fs-4 fw-normal m-0">{{ post.preview }}</p>
              </div>	      
            </article>
          </a>       
        {% endfor %}
      </div>
  </div>

  <style>
    .post-preview 
    {
        border-radius: 25px;
        width: 33%;
        aspect-ratio: 16 / 9;
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