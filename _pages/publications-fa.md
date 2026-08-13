---
layout: page
permalink: /fa/publications/
title: مقالات
page_id: publications
lang: fa
lang_ref: publications
description: فهرست کامل مقالات بر اساس گوگل اسکالر، به ترتیب زمانی معکوس.
years: [2026, 2025, 2024, 2023, 2022, 2020, 2019, 2018, 2014]
nav: true
nav_order: 2
---

<p>پروفایل کامل در <a href="https://scholar.google.com/citations?user=mZzvI4MAAAAJ&hl=en" target="_blank" rel="noopener">گوگل اسکالر</a>.</p>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
