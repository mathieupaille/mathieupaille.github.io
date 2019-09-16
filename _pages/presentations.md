---
layout: page
permalink: /presentations/
title: presentations
description: 
years: [2019,2018,2017,2016]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}
