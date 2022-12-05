---
layout: page
permalink: /publications/
title: <b>Research</b>
description: Here's what I have been working on...
years: [1967, 1956, 1950, 1935, 1905]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<font size="5"><b> Journal Articles </b></font>   
  {% bibliography %}
  
<font size="5"><b> Working Papers </b></font>  
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
  
<font size="5"><b> Work-In-Progress </b></font>   
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
  
  
</div>
