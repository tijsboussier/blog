---
layout: page
title: "Changelog"
permalink: /changelog
---

{% for changelog in site.changelog %}
  <ul>
    <li>
      <a href="{{ changelog.url }}">
        {{ changelog.title | markdownify }}
      </a>
    </li>
  </ul>
{% endfor %}
