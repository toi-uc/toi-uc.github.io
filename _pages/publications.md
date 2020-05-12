---
layout: page
permalink: /publications/
title: publications
description: Papers I have authored (still incomplete, wait for update...)
years: [2020, 2019, 2018, 2017, 2016]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
