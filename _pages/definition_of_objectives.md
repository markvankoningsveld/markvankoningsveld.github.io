---
layout: page
title: Definition of objectives
permalink: /definition_of_objectives
category: [Frame of Reference]
---

According to the <a href="https://www.merriam-webster.com/dictionary/objective">Webster dictionary</a> an objective is 'something toward which effort is directed: an aim, goal, or end of action'. The Frame of Reference distinguishes two levels of objectives: the strategic objective and the operational objective.
 
A strategic objective is a long-term, often vision related, goal that provides a guiding context for the development of more specific plans and projects. An operational objective is a specification of the strategic objective. It specifies what type of action is undertaken to achieve (part of) the strategic objective. A properly formulated operational objective: 
<ul>
    <li>identifies a specific thing that you want to direct effort to,</li>
    <li>identifies a specific target that you are striving for,</li>
    <li>expresses an observable verb that describes the behavior that you are striving for,</li>
    <li>specifies additional criteria to indicate how or when the outcome will be observable.</li>
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
