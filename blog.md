---
layout: default
title: My Blog
permalink: /blog/
---

<h1 class="text-center title">{{ page.title | escape }}</h1>
<hr class="title">

{% if site.posts.size == 0 %}

  <h6>There is nothing you can read at the moment, but I am writing. Come later!</h6>

{% else %}

{% for post in site.posts %}

  <div class="card border-secondary post-card">
    <div class="card-header bg-secondary border-secondary">
      <h3 class="card-title text-white">{{ post.title | escape }}</h3>
      <h6 class="card-subtitle mb-2">
        <span class="blog-date">{{ post.date | date_to_long_string }}</span>
        {% for tag in post.tags %}

        <span class="badge badge-primary post-tag">{{ tag }}</span>

        {% endfor %}
      </h6>
    </div>
    <div class="card-body">
      <p class="card-text">
        {{ post.description | escape }}
      </p>
      <h6 class ="text-center">
        <a href="{{ post.url | relative_url }}" class="no-link">~ Continue reading ~</a>
      </h6>
    </div>
  </div>

{% endfor %}

{% include license.html %}

{% endif %}
