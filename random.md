---
layout: page
title: Random
permalink: /random/
---

{% for post in site.categories.random %}
  <article>
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %} 