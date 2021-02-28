---
layout: page
permalink: /publications/
title: publications
description: My published research from undergrad and beyond
years: [2020, 2019, 2017, 2014]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
