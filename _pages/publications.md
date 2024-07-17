---
layout: page
permalink: /publications/
title: publications
description: 
years: [to appear, 2024, 2023, 2022, 2021, 2020, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h1 class="year">{{y}}</h1>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
