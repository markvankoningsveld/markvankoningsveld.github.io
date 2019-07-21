---
layout: page
title: Sustainable Infrastructure
permalink: /sustainable_infrastructure
---

Mankind develops and operates all sorts of infrastructure to meet societies needs more efficiently. With the growing world population mankinds drive to modify the natural system needs to be assessed for its long term sustainability. Laboyrie et al. (2018) collected best practices from the marine construction industry related to this topic.

<img src="assets/images/Dredging_for_Sustainable_Infrastructure.png" alt="Dredging for Sustainable Infrastructure">

<!-- Posts Index
================================================== -->
<section class="recent-posts">

    <div class="row listrecent">
    <div class="section-title col-md-12 mt-4">
    <h2 id="{{ site.categories{'software'}[0] | replace: " ","-" }}">Category <span class="text-capitalize">{{ site.categories{'software'}[0] }}</span></h2>
    </div>
    {% assign pages_list = category[1] %}
    {% for post in pages_list %}
    {% if post.title != null %}
    {% if group == null or group == post.group %}
    {% include postbox.html %}
    {% endif %}
    {% endif %}
    {% endfor %}
    {% assign pages_list = nil %}
    {% assign group = nil %}
    </div>

</section>