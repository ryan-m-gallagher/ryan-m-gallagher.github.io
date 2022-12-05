---
layout: page
permalink: /publications/
title: Research
description: Here's what I have been working on...
years: [1967, 1956, 1950, 1935, 1905]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<font size="6"><b> Journal Articles </b></font> 
  
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<b> Working Papers </b> 
  
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
  
<b> Works in Progress </b> 
  
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
  
  
</div>
