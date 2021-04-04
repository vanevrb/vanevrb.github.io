---
layout: page
title: Blog
permalink: /blog/
---

<div class="container">
    <div class="row">
       {% for post in site.posts %}
        <div class="col-6 col-sm-4">
            <div class="card mr-3">
                <img src="./img/posts/1.png" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</h5>
                    <p class="card-text">
                       {{ post.excerpt }}</p>
                    <a href="{{ site.baseurl }}{{ post.url }}" class="btn btn-primary">Ver más</a>
                </div>
            </div>
        </div>
       {% endfor %}
    </div>
</div>
