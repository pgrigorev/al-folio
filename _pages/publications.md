---
layout: page
permalink: /publications/
title: publications
description:
years: [2021, 2020, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
---

A pdf version of the publication list can be downloaded here: <a href="/assets/pdf/Publication_list_Grigorev.pdf" target="_blank" title="download list of publications"> <i class="far fa-file-pdf" aria-hidden="true"></i> list of publications</a>.

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
