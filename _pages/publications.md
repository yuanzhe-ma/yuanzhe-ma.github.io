---
layout: page
permalink: /publications/
title: publications
description:  
years: [2022]
nav: true
---

<div class="publications">
<a href="https://scholar.google.com/citations?user=4d8UV8sAAAAJ">Google Scholar</a>  

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
