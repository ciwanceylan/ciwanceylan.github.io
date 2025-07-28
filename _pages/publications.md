---
layout: page
permalink: /publications/
title: publications
description: 
years_publications: [2025, 2024, 2021, 2018]
years_preprint: [2022]
nav: true
---

<div class="publications">

{% for y in page.years_publications %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div class="preprints">

{% for y in page.years_preprint %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f preprints -q @*[year={{y}}]* %}
{% endfor %}

</div>
