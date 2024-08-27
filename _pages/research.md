---
layout: page
permalink: /research/
title: research
description: Papers and publications
years: [2021, 2020, 2016]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
