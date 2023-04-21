---
layout: page
permalink: /publications/
title: publications
description:
years: [2023, 2022, 2021, 2020, 2018]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

An up-to-date list is available on <a href="https://scholar.google.com/citations?user=OdzPaPIAAAAJ&hl=en&oi=ao">Google Scholar</a>.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
