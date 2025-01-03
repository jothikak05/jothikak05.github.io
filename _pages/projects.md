---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

<div style="display: flex; flex-wrap: wrap; gap: 20px; margin-top: 15px;">
  
  {% for project in site.projects %}
    <div style="width: 300px; border: 1px solid #ccc; border-radius: 10px; overflow: hidden; background-color: #f9f9f9;">
      <a href="{{ project.url }}">
        <img src="{{ project.image }}" alt="{{ project.title }}" style="width: 100%; height: 200px; object-fit: cover; border-bottom: 1px solid #ccc;">
        <div style="padding: 15px;">
          <h3 style="font-size: 18px; margin: 0;">{{ project.title }}</h3>
          <p style="font-size: 14px; color: #555;">{{ project.excerpt | strip_html | truncatewords: 20 }}</p>
        </div>
      </a>
    </div>
  {% endfor %}

</div>
