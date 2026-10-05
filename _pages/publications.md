---
published: false # publications now live on the research page
layout: page
permalink: /publications/
title: Publications
description: Published and submitted papers. Work in preparation is listed on the research page.
years: [2026, 2025, 2023]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
