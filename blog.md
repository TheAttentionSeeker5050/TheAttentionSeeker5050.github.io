---
layout: default
title: Blog
permalink: /blog
---

# Blog

{% if site.posts.size == 0 %}
  No posts available.
{% else %}
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
{% endif %}