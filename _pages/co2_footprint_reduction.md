---
layout: page
title: CO2 footprint reduction
permalink: /co2_footprint_reduction
category: [CO2 footprint reduction]
---

One of the sustainability initiatives that I am involved with is the development of innovative technologies for CO2 footprint reduction. 

{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
