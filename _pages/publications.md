---
layout: page
permalink: /publications/
title: Publications
description: Selected Publications. Unfortunately due to the sensitive nature of the data contained in other projects, they are unpublished .
years: [2023, 2021, 2020]
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
