---
layout: default
title: Portfolio
permalink: /portfolio/
---

# Portfolio

{% if site.portfolio.size == 0 %}
  No portfolio entries available.
{% else %}
  <ul id="portfolio-list-items">
    {% for project in site.portfolio %}
      <li>
        <a href="{{project.url}}">{{project.title}}</a>
      </li>
    {% endfor %}
  </ul>
{% endif %}