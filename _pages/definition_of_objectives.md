---
layout: page
title: Definition of objectives
permalink: /definition_of_objectives
category: [Frame of Reference]
---

According to the <a href="https://www.merriam-webster.com/dictionary/objective">Webster dictionary</a> an objective is 'something toward which effort is directed: an aim, goal, or end of action'.

{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
