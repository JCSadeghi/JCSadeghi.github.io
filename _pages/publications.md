---
layout: page
permalink: /publications/
title: publications and conference talks
description: Selected Papers and Talks
yearst: [2020]
yearsj: [2021,2019,2016]
yearsr: [2019]
yearsc: [2018,2017]
---
### Thesis:
{% for y in page.yearst %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f thesis -q @*[year={{y}}]* %}
{% endfor %}
### Papers:
{% for y in page.yearsj %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
### Technical Reports:
{% for y in page.yearsr %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f reports -q @*[year={{y}}]* %}
{% endfor %}
### Conference Papers/Talks:
{% for y in page.yearsc %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}
