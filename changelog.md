---
layout: page
title: "Changelog"
permalink: /changelog
---
Recent updates. For a full history, check [below](#history).

{% assign changelog = site.changelog %}
  {{ changelog.last.content}}

## History

<ul>
  {% for changelog in site.changelog reversed %}
      <li><a href="{{ changelog.url }}">{{ changelog.name | markdownify }}</a></li>
  {% endfor %}
</ul>
