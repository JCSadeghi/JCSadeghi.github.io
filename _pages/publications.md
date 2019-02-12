---
layout: page
permalink: /publications/
title: publications and conference talks
description: Selected Papers and Talks
yearsj: [2019,2018,2016]
yearsc: [2018,2017]
---
### Journal Papers:
{% for y in page.yearsj %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
### Conference Papers/Talks:
{% for y in page.yearsc %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}
