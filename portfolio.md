---
layout: default
title: Portfolio
permalink: /portfolio/
---

<div id="portfolio-list-container">
  <h1>Portfolio</h1>
  {% if site.portfolio.size == 0 %}
    <p>No portfolio entries available.</p>
  {% else %}
    <ul id="portfolio-list-items">
      {% for project in site.portfolio %}
        <li>
          <a href="{{project.url}}" class="portfolio-item-link">
            {% if project.thumbnail %}
              <img src="{{project.thumbnail}}" alt="{{project.title}}">
            {% else %}
              <img src="https://placehold.co/200x150?text=Project+Thumbnail" alt="{{project.title}}"/>
            {% endif %}
            <div class="github-repo-link-wrapper">
              <h2>{{project.title}}</h2>
              {% if project.repository %}
                <p>Has GitHub repository</p>
              {% else if project.backendRepository or project.frontendRepository %}
                <p>Has separate GitHub repositories for backend and frontend</p>
              {% else %}
                <p>GitHub repository not fount</p>
              {% endif %}
              {% if project.liveDemo %}
                <p>Has live demo</p>
              {% endif %}
            </div>
          </a>
        </li>
      {% endfor %}
    </ul>
  {% endif %}
</div>