---
layout: page
title: East Meets West
permalink: /east-meets-west/
---

When I started writing East Meets West, I was -- and still am -- very interested in the tech industry in Asia. In the years leading up to beginning East Meets West, I had the opportunity to spend a lot of time living and working throughout Asia and always found it so surprising how isolated and understudied the tech industry in Asia was.
As the "West" in East Meets West, I wanted to bring an outsider perspective to the companies and entrepreneurs in Asia.

I felt many people's views of tech in China and other Asia conutries was informed by Peter Thiel's Zero to One quote, "The easiest way for China to grow is to relentlessly copy what has already worked in the West."

At some point, that was true. However, I don't think it is anymore. Western technology companies, especially those focused on consumers, are now looking to China and Southeast Asia to copy ideas from Asia's best entrepreneurs.

As of 2021, I stopped writing about East Meets West. While I still read and learn about the tech industry in Asia, I don't have the time to write about it anymore as all my attention has refocused to crypto markets and my company, [Wallfacer Labs](/about)



![East Meets West Banner](/assets/emwlong.png)

{% for post in site.categories.east-meets-west %}
  <article>
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </article>
{% endfor %} 