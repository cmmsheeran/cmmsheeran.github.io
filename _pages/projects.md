---
layout: page
title: research
permalink: /research/
description: Research interests and current projects.
nav: true
nav_order: 1
horizontal: true
---

The overarching purpose of my research is in the elucidation of _scale_, most generally in complex systems but more specifically in the brain. 
My current work develops this programme along three closely related directions:

## Mesoscale structure and observables
### What is a mesoscale structure, and how does it constrain dynamics?
### blah blah

## Coarse-graining and emergence
### General network renormalization
### A mechanism of emergence: Closure-defects and the emergent phenomena.  

### Collective organization (Ranking)

---

## Current projects

<div class="projects">
{% if site.enable_project_categories and page.display_categories %}

  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>

  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}

  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}

  {% endfor %}

{% else %}

  {% assign sorted_projects = site.projects | sort: "importance" %}

  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}

{% endif %}
</div>
