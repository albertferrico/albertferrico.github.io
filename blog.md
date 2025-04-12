---
layout: default
title: Blog
permalink: /blog.html
---

# Blog

{% for post in site.posts %}
  <div class="post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="date">{{ post.date | date: "%d %B %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </div>
{% endfor %}