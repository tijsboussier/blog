---
layout: page
permalink: /then/
title: "What I Was Doing Then"
---
This is an archive of my <a href="https://nownownow.com/about" target="_blank">Now-pages</a>.
  
{% assign my_then_order = site.then | sort | reverse %}
  <ul>
  {% for then in my_then_order %}
      <li><a href="{{ then.url }}">{{ then.name }}</a></li>
  {% endfor %}
</ul>
