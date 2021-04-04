---
layout: default
---


ruta
<h2>{{ site.posts[0].title }}</h2>
<div class="row">
                            <div class="col-12 col-md-6 col-xl-3 mb-4">
                                <div class="card mr-3">
                                    <img src="{{ site.baseurl }}/assets/img/posts/{{ site.posts[0].image }}.png" class="card-img-top" alt="...">
                                    <div class="card-body">
                                      <h5 class="card-title">{{ site.posts[0].title }}</h5>
                                      <p class="card-text">We’re getting nearer to the end of summer and because we know that this period can make a serious dent in your pocket..</p>
                                      <a href="#" class="btn btn-primary">Read more</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-12 col-md-6 col-xl-3 mb-4">
                                <div class="card mr-3">
                                    <img src="https://themesberg.s3.us-east-2.amazonaws.com/public/posts/gpt-3-tailwind-css-code-generator.jpg" class="card-img-top" alt="...">
                                    <div class="card-body">
                                      <h5 class="card-title">We built an OpenAI powered Tailwind CSS code generator using GPT-3</h5>
                                      <p class="card-text">A couple of days ago we got access to the OpenAI’s Beta API platform and I had the occasion to play around with it...</p>
                                      <a href="#" class="btn btn-primary">Read more</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-12 col-md-6 col-xl-3 mb-4">
                                <div class="card mr-3">
                                    <img src="https://themesberg.s3.us-east-2.amazonaws.com/public/posts/bootstrap-5-tutorial/bootstrap-5-tutorial.jpg" class="card-img-top" alt="...">
                                    <div class="card-body">
                                      <h5 class="card-title">Bootstrap 5 tutorial: learn how to get started without jQuery</h5>
                                      <p class="card-text">We’re getting nearer to the end of summer and because we know that this period can make a serious dent in your pocket..</p>
                                      <a href="#" class="btn btn-primary">Read more</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-12 col-md-6 col-xl-3 mb-4">
                                <div class="card mr-3">
                                    <img src="https://themesberg.s3.us-east-2.amazonaws.com/public/posts/angular-10/angular-10-officially-released-dropping-ie-9-10.jpg" class="card-img-top" alt="...">
                                    <div class="card-body">
                                      <h5 class="card-title">Angular 10 officially released deprecating support for IE 9 and 10</h5>
                                      <p class="card-text">If you’ve been using Angular for your web projects I’m glad to let you know that following this major update to version...</p>
                                      <a href="#" class="btn btn-primary">Read more</a>
                                    </div>
                                </div>
                            </div>
                        </div>
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

