---
layout: page
title: East Meets West
permalink: /east-meets-west/
---

When I started writing East Meets West, I was – and still am – very interested in the tech industry in Asia. After spending years living and working throughout the region, I found it surprising how isolated and understudied its tech industry was. As the "West" in East Meets West, I wanted to bring an outsider perspective to these companies and entrepreneurs.

I felt many people's views of tech in Asia were shaped by Peter Thiel's Zero to One quote: "The easiest way for China to grow is to relentlessly copy what has already worked in the West." While this was true at some point, it isn't anymore. Today, Western technology companies, especially those focused on consumers, are looking to China and Southeast Asia to copy ideas from Asia's best entrepreneurs.

As of 2021, I stopped writing about East Meets West as my attention refocused on crypto markets and my company, [Wallfacer Labs](/about). Though I still follow the Asian tech industry, I no longer have time to write about it.



![East Meets West Banner](/assets/emwlong.png)

{% for post in site.categories.east-meets-west %}
  <article>
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %} 