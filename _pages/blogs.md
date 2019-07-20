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

        {% for post in paginator.posts %}

        {% include postbox.html %}

        {% endfor %}

    </div>

</section>

</div>

<div class="col-md-4">

</div>
</div>
