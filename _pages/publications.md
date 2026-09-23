---
layout: page
permalink: /publications/
title: Publications
description: Research on uncertainty-aware learning, evidential models, and adapting foundation models with limited data.
years: [2026, 2024, 2023, 2022, 2021]
nav: true
nav_order: 1
---

<div class="publications">
{% for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

For the complete record, see my [Google Scholar profile](https://scholar.google.com/citations?user=EGkWnakAAAAJ).
