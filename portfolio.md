---
layout: default
title: Portfolio
permalink: /portfolio/
---

# Portfolio

<ul id="portfolio-list-items">
{% for project in site.portfolio %}
  <li>
    <a href="{{project.url}}">{{project.title}}</a>
  </li>
{% endfor %}
</ul>