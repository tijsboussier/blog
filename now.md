---
layout: page
permalink: /now
title: "What I'm Doing Now"
navlink: Now
---

{% assign my_then_order = site.then | sort | reverse %}
  This is my [Now-page](https://nownownow.com/about), inspired by [Derek Sivers](https://sive.rs/). Last updated on {{ my_then_order.first.date | date: '%e %B %Y' }}.

  {{ my_then_order.first.content }}
