---
layout: page
title: Reef rehabilitation
permalink: /reef_rehabilitation
category: [Reef rehabilitation]
---

One of the sustainability initiatives that I am involved with is the development of innovative technologies for active reef rehabilitation. 

{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
