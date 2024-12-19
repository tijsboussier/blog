---
layout: page
title: "Changelog"
permalink: /changelog
---
<p class="infobox">Recent updates. For a full history, check <a href="#history">below</a>.</p>

{% assign changelog = site.changelog %}
  {{ changelog.last.content}}

<h2 class="top-bordered" id="history">History</h2>

<ul>
  {% for changelog in site.changelog offset:1 %}
      <li><a href="{{ changelog.url }}">{{ changelog.name }}</a></li>
  {% endfor %}
</ul>
