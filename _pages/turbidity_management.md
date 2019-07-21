---
layout: page
title: Turbidity management
permalink: /turbidity_management
category: [Turbidity management]
---

One of the sustainability initiatives that I am involved with is the development of innovative technologies for turbidity management. 

<img src="assets/images/PlumeGuard.png" alt="Innovative turbidity monitoring frame">

{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
