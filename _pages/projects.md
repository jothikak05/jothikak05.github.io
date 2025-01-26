---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center; margin-top: 15px;">

  {% for project in site.projects %}
    <div style="width: 300px; border: 1px solid #ddd; border-radius: 12px; overflow: hidden; background-color: #fff; box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1); transition: transform 0.3s ease, box-shadow 0.3s ease;" onmouseover="this.style.transform='scale(1.05)'; this.style.boxShadow='0 10px 20px rgba(0, 0, 0, 0.15)';" onmouseout="this.style.transform='scale(1)'; this.style.boxShadow='0 6px 12px rgba(0, 0, 0, 0.1)';">
      <a href="{{ project.url }}" style="text-decoration: none; color: inherit; display: block;">
        <img src="{{ project.image }}" alt="{{ project.title }}" style="width: 100%; height: 200px; object-fit: cover; border-bottom: 1px solid #ddd;">
        <div style="padding: 20px; text-align: center;">
          <h3 style="font-size: 18px; margin: 0; color: rgb(31, 85, 193); font-weight: 600;">{{ project.title }}</h3>
        </div>
      </a>
    </div>
  {% endfor %}

</div>
