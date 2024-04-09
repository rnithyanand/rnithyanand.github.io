---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024,2023,2022,2020,2018,2017,2016,2014,2013,2012,2011,2010]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
 <!-- <h2 class="year">{{y}}</h2>-->
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
