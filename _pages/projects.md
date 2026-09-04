---
layout: page
title: research
permalink: /research/
nav: true
nav_order: 1
horizontal: true
---

My work is organized around a central question:

> **What is SCALE?**


---

## Current projects

<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
  </div>
</div>
