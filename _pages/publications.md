---
layout: page
permalink: /publications/
title: Publications
description: <span>&#42;</span> indicates equal contribution
years: [2021]
nav: true
importance: 1
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  <br>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
