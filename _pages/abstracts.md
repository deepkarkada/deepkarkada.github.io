---
layout: page
permalink: /abstracts/
title: abstracts
description: Abstracts by categories in reversed chronological order. generated by jekyll-scholar.
years: [2021, 2020, 2019, 2018]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="abstracts">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>