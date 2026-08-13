---
layout: page
permalink: /fa/projects/
title: پژوهش
page_id: projects
lang: fa
lang_ref: projects
description: محورهای پژوهشی در تربیت معلم و یادگیری زبان با پشتیبانی فناوری.
nav: true
nav_order: 4
horizontal: false
---

<div class="projects">
  {%- assign lang_projects = site.projects | where: "lang", "fa" -%}
  {%- assign sorted_projects = lang_projects | sort: "importance" -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
</div>
