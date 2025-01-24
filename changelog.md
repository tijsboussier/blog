---
layout: page
title: "Changelog"
permalink: /changelog/
---
## Recent updates

{% assign my_changelog_order = site.changelog | sort | reverse %}
  {{ my_changelog_order.first.content }}

## History

<ul>
  {% for changelog in my_changelog_order offset:1 %}
      <li><a href="{{ changelog.url }}">{{ changelog.name }}</a></li>
  {% endfor %}
</ul>
