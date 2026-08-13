---
layout: page
permalink: /fa/publications/
title: مقالات
page_id: publications
lang: fa
lang_ref: publications
description: فهرست مقالات به ترتیب زمانی معکوس.
years: [2024, 2020, 2018]
nav: true
nav_order: 2
---

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
