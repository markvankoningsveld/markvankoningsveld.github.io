---
layout: page
title: Sustainable Infrastructure
permalink: /sustainable_infrastructure
category: [Sustainability, Reef rehabilitation, CO2 footprint reduction, Turbidity management]
---

Mankind develops and operates all sorts of infrastructure to meet societies needs more efficiently. With the growing world population mankinds drive to modify the natural system needs to be assessed for its long term sustainability. Laboyrie et al. (2018) collected best practices from the marine construction industry related to this topic.

<img src="assets/images/Dredging_for_Sustainable_Infrastructure.png" alt="Dredging for Sustainable Infrastructure">

{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

