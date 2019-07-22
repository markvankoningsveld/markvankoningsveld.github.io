---
layout: page
title: Definition of objectives
permalink: /definition_of_objectives
category: [Frame of Reference]
---

According to the <a href="https://www.merriam-webster.com/dictionary/objective">Webster dictionary</a> an objective is 'something toward which effort is directed: an aim, goal, or end of action'.

The Frame of Reference distinguishes two levels of objectives: the strategic objective and the operational objective.

Van Koningsveld and Mulder (2004) defined a basic frame of reference including an operational objective. During the CONSCIENCE project some arguments were made to rename this level of objectives to tactical objective. More important than the exact name is the elements that should be included in a properly formulated operational objective. AVan Koningsveld and Mulder (2004) defined a basic frame of reference including an operational objective. During the CONSCIENCE project some arguments were made to rename this level of objectives to tactical objective. More important than the exact name is the elements that should be included in a properly formulated operational objective. A Van Koningsveld and Mulder (2004) defined a basic frame of reference including an operational objective. During the CONSCIENCE project some arguments were made to rename this level of objectives to tactical objective. More important than the exact name is the elements that should be included in a properly formulated operational objective. A properly formulated operational objective: 
<ul>
    <li>identify a specific thing that you want to direct effort to, 
    <li>identify a specific target that you are striving for,
    <li>select an observable verb that describe the behavior that you are striving for,
    <li>add additional criteria to indicate how or when the outcome will be observable.
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
