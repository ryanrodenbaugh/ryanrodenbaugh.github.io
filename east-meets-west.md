---
layout: page
title: East Meets West
permalink: /east-meets-west/
---

![East Meets West Banner](emwlong.png)

I was -- and still am -- very interesed in the tech industry in Asia. While many

{% for post in site.categories.east-meets-west %}
  <article>
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %} 