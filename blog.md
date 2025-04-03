---
layout: default
title: "Blog"
permalink: /blog/
body_class: blog-page
---
{% include header_dml.html %}

<section class="devlog-container">
  <div class="container d-flex flex-column" style="padding: 100px 0 150px 0; row-gap: 50px">
    <div class="section-header text-center">
      <h1 class="fs-1 fw-bold text-uppercase text-white m-0">Blog</h1>
    </div>

    <div class="row g-5 m-0">
        {% for post in site.posts %}
	  <div class="col col-md-4 d-flex m-0">
            <a class="text-decoration-none text-white m-0 p-0" href="{{ post.url }}">
              <article class="post-preview">
                <img class="img-fluid post-banner" style="border-radius: 20px 20px 0 0; width: 100%; aspect-ratio: 16 / 9" src="{{ post.banner }}">

                <div class="col d-flex p-3 p-md-5" style="flex-direction: column">         
                  <p class="fs-5 fw-normal mb-3 p-0" style="color: #92dce5">{{ post.date | date: "%B %d, %Y" }}</p>   
                  <h2 class="fs-3 fw-bold mb-3 p-0">{{ post.title }}</h2>                         
                  <p class="fs-5 fw-normal m-0">{{ post.preview }}</p>
                </div>	      
              </article>
            </a>  
          </div>     
        {% endfor %}   
      </div>
  </div>

  <style>
    .post-preview 
    {
        border-radius: 20px;
	height: 100%;
        width: 100%;
        background-color: #6A2388;
        box-shadow: 0px 0px 15px 5px rgba(0, 0, 0, 0.25);
        transition: box-shadow 0.3s ease-in-out;
    }

    .post-preview:hover 
    {
        box-shadow: 0px 0px 30px 5px rgba(146, 220, 229, 0.50);
    }
  </style>
</section>