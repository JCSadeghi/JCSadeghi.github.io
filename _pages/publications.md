---
layout: page
permalink: /publications/
title: publications
description: Publications, patents, technical reports, thesis, and conference papers.
nav: true
nav_order: 2
yearst: [2020]
yearsj: [2026, 2024, 2023, 2022, 2021, 2019, 2016]
yearsr: [2026, 2019]
yearsc: [2018, 2017]
---

I am a named inventor on granted patents covering perception uncertainty, perception error modelling, and simulation-based testing ([Espacenet](https://worldwide.espacenet.com/patent/search/family?q=in%20%3D%20%22SADEGHI%20JONATHAN%22)).

### Papers:

{% for y in page.yearsj %}

  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
### Thesis:
{% for y in page.yearst %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f thesis -q @*[year={{y}}]* %}
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
