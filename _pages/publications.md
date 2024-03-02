---
layout: page
permalink: /publications/
title: Publications
description: Erez Yosef publications in reversed chronological order. <a href='https://scholar.google.com/citations?user=NOIkjY8AAAAJ&hl'>Google Scholar</a>. \n <a href="https://scholar.google.com/citations?user={{ site.scholar_userid }}" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
years: [2024, 2023, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
