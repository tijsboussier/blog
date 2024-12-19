---
layout: page
title: "Changelog"
permalink: /changelog
---
Recent updates. For a full history, check [here](#history).

{% for changelog in site.changelog limit:1 %}
  {{ changelog.content}}
{% endfor %}

## History

<ul>
  {% for changelog in site.changelog reversed %}
      <li><a href="{{ changelog.url }}">{{ changelog.name | markdownify }}</a></li>
  {% endfor %}
</ul>
