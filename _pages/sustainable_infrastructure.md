---
layout: page
title: Sustainable Infrastructure
permalink: /sustainable_infrastructure
category: software
---

Mankind develops and operates all sorts of infrastructure to meet societies needs more efficiently. With the growing world population mankinds drive to modify the natural system needs to be assessed for its long term sustainability. Laboyrie et al. (2018) collected best practices from the marine construction industry related to this topic.

<img src="assets/images/Dredging_for_Sustainable_Infrastructure.png" alt="Dredging for Sustainable Infrastructure">

{% for cat in site.categories %}
    <li>{{ cat[0] }}</li>
{% endfor %}

{% for post in site.categories.CATEGORY_NAME %}
    <li>{{ post }}</li>
{% endfor %}

{% assign cat = page.category %}
<div class="category-archive">
  <div>
    <span class="title">Category archive for {{ cat }}</span>
  </div>
  <div>
    {{ cat }}
    <ul class="posts">
      {% for post in site.categories.cat %}
      <li><span>{{ post.date | date_to_string }} - </span> <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </div>
</div>