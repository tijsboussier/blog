---
layout: page
title: "Changelog"
permalink: /changelog
---
<p class="infobox">Recent updates. For a full history, check <a href="#history">below</a>.</p>

{% assign my_changelog_order = site.changelog | sort | reverse %}
  {{ my_changelog_order.first.content}}

<h2 class="top-bordered" id="history">History</h2>

<ul>
  {% for changelog in my_changelog_order offset:1 %}
      <li><a href="{{ changelog.url }}">{{ changelog.name }}</a></li>
  {% endfor %}
</ul>
