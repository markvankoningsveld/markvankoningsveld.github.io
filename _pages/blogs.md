---
layout: page
title: Blogs
permalink: /blogs
---

<div class="row justify-content-between">
<div class="col-md-8 pr-5">

<!-- Posts Index
================================================== -->
<section class="recent-posts">

    <div class="section-title">

        <h2><span>All Stories</span></h2>

    </div>

    <div class="row listrecent">
    {% for category in site.categories %}
    <div class="section-title col-md-12 mt-4">
    <h2 id="{{ category[0] | replace: " ","-" }}">Category <span class="text-capitalize">{{ category[0] }}</span></h2>
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
    {% endfor %}
    </div>

</section>

</div>

<div class="col-md-4">

</div>
</div>
