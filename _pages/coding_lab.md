---
layout: page
title: Ports and Waterways Coding Lab
permalink: /coding_lab
category: [Software, Ports & Waterways Coding Lab]
---

The Ports and Waterways chair at TU Delft is dedicated to deliver excellent academic research and education on the analysis, design and management of competitive, safe and sustainable waterborne supply chains.

<img src="assets/images/Ports_and_Waterways.png" alt="Ports and Waterways system overview">

Design of Ports and Waterways systems is a complex challenge that requires simulation and economic evaluation to support decision making, especially when non-linear feedbacks make it impossible to rely on intuition.

The Ports and Waterways discipline focuses on the effective analysis, design and management of (water) infrastructure (system as a whole and/or its individual system elements), while considering:
<ul>
  <li>nautical traffic (nodes and edges or free routing)</li>
  <li>logistical processes (cargo)</li>
  <li>environmental/physical conditions (natural, man made)</li>
  <li>engineering knowledge (energy use, sound, spill, etc.)</li>
</ul>

Analyses should go beyond one single-objective business case (although this is an important base case). Different stakeholders find different aspects important. An integral approach is needed.


{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}