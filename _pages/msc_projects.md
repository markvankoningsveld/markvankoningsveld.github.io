---
layout: page
title: MSc projects
permalink: /msc_projects
category: [MSc Thesis]
---

See below a list of MSc projects I was involved in. 

{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
