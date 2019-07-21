---
layout: page
title: Sustainable Infrastructure
permalink: /sustainable_infrastructure
category: [Software]
---

Mankind develops and operates all sorts of infrastructure to meet societies needs more efficiently. With the growing world population mankinds drive to modify the natural system needs to be assessed for its long term sustainability. Laboyrie et al. (2018) collected best practices from the marine construction industry related to this topic.

<img src="assets/images/Dredging_for_Sustainable_Infrastructure.png" alt="Dredging for Sustainable Infrastructure">

<h3>{{ page.category }}</h3>

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

{% for category in site.categories %}
  {% if post.categories contains "Software" %}
    <h3>{{ category[0] }}</h3>
    <ul>
      {% for post in category[1] %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  {% endif %}  
{% endfor %}

