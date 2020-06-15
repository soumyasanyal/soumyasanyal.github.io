---
layout: page
permalink: /publications/
title: Publications
description: <a style="color:#00369f;" href="https://www.semanticscholar.org/author/Soumya-Sanyal/3313909">[Semantic Scholar</a> | <a style="color:#00369f;" href="https://scholar.google.com/citations?user=KvaizyQAAAAJ&hl=en">Google Scholar]</a>
years: [2020, 2019, 2018]
footnote: "* Equal contribution"
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
