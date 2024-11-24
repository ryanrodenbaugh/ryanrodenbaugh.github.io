---
layout: page
title: East Meets West
permalink: /east-meets-west/
---

{% for post in site.categories.east-meets-west %}
  <article>
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %} 