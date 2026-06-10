---
layout: page
permalink: /then/
title: "What I Was Doing Then"
---
<p class="infobox">
This is an archive of my <a href="https://nownownow.com/about" target="_blank">Now-pages</a>.<br />
Go to <a href="{{site.baseurl}}/now">current Now-page</a> instead.
</p>

{% assign my_then_order = site.then | sort | reverse %}
  <ul>
  {% for then in my_then_order %}
      <li><a href="{{ then.url }}">{{ then.name }}</a></li>
  {% endfor %}
</ul>
