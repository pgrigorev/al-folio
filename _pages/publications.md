---
layout: page
permalink: /publications/
title: publications
description:
years: [2024, 2023, 2022, 2021, 2020, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
nav_order: 1
---

A pdf version of the full list of publications can be downloaded here: <a href="/assets/pdf/Publication_list_Grigorev.pdf" target="_blank" title="download list of publications"> <i class="far fa-file-pdf" aria-hidden="true"></i> list of publications</a>.

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
