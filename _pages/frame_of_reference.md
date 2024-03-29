---
layout: page
title: Frame of Reference
permalink: /frame_of_reference
category: [Frame of Reference]
---

The Frame of Reference approach provides a generic approach to value assessment and management. Key to the approach is to make important aspects of a management issue explicit to facilitate interaction between actors with different backgrounds. An important question is which elements should be made explicit as a minimum.

<img src="assets/images/Frame_of_Reference.png" alt="Basis Frame of Reference template">

Based on an analysis of the successful Dutch 'Dynamic Preservation' policy for coastal sediment management, it was proposed that a 'basic' frame of reference should at least include:
<ul>
  <li>A strategic objective;</li>
  <li>An operational objective; and</li>
  <li>A decision recipe containing a foursome of elements, viz.:</li>
  <ul>
    <li>A quantitative state concept;</li>
    <li>A benchmarking procedure;</li>
    <li>An intervention procedure; and</li>
    <li>An evaluation procedure confronting the operational as well as the
        strategic objective.</li>
  </ul>
</ul>


{% for category in page.category %}
  <h4>Posts on {{ category }}:</h4>
  {% assign cat = category %}
  <ul>
    {% for post in site.categories.[cat] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
