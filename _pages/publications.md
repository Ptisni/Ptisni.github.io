---
layout: page
permalink: /publications/
title: Publications
description: All publications are also available on my Google Scholar. * Denotes equal contribution.
years: [2024, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
