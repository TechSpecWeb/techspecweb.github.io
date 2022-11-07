---
layout: default
title: News
---
<h1>Uutiset</h1>

<ul>
  {% for post in site.posts %}
    <li class="news-header">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {% for category in post.categories %}
        <span class="category-tag">{{ category }}</span>
      {% endfor %}
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>