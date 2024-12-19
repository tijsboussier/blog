---
layout: page
permalink: /then
title: "What I Was Doing Then"
navlink: Now
---

{% assign my_then_order = site.then | sort | reverse %}
  <ul>
  {% for then in my_then_order offset:1 %}
      <li><a href="{{ then.url }}">{{ then.name }}</a></li>
  {% endfor %}
</ul>
