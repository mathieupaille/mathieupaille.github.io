---
layout: page
permalink: /presentations/
title: presentations
description: 
years: [2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}

</div>