---
layout: page
permalink: /publications/
title: Publications
page_id: publications
lang: en
lang_ref: publications
description: Complete list of publications from Google Scholar, in reverse chronological order.
years: [2026, 2025, 2024, 2023, 2022, 2020, 2019, 2018, 2014]
nav: true
nav_order: 2
---

<p>Full profile on <a href="https://scholar.google.com/citations?user=mZzvI4MAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>.</p>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
