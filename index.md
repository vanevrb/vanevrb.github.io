---
layout: default
---


ruta
<h2>{{ site.posts[0].title }}</h2>

<div id="main" role="main" class="container">

    <div class="row">
        <div class="col-sm-3">
            <ul class="nav flex-column">
                <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="#">Active</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
                </li>
            </ul>
        </div>
        <div class="col-sm-9">

            <div class="row">

                {% for post in site.posts %}
                <div class="col-sm-12">
                    <div class="card">
                        <div class="card-body">
                            <h5 class="card-title">
                                <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
                            </h5>
                            {% if post.image %}
			    	{{ post.image }}
			    {% endif %}
			    <h1 class="headline">{{ post.title }}</h1>
                            <p class="card-text"> {{ post.excerpt }}</p>
                            <a href="{{ site.baseurl }}{{ post.url }}" class="btn btn-primary">Read More</a>
                        </div>
                    </div>
                </div>
                {% endfor %}
            </div>
        </div>
    </div>
</div>

