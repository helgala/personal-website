---
layout: page
title: projects
permalink: /projects/
description: Selected research and academic initiatives led or supported by Hany Elgala.
nav: true
nav_order: 2
---

Selected research and academic initiatives led or supported by Hany Elgala.

<div class="row row-cols-1 row-cols-md-3">
  {% assign projects = site.projects | sort: "importance" %}
  {% for project in projects %}
    <div class="col mb-4">
      <a href="{{ project.external_url | default: project.url | relative_url }}"{% if project.external_url %} target="_blank" rel="noopener"{% endif %}>
        <div class="card hoverable h-100">
          {% if project.img %}<img src="{{ project.img | relative_url }}" class="card-img-top" alt="{{ project.title }} preview">{% endif %}
          <div class="card-body"><h2 class="card-title">{{ project.title }}</h2><p class="card-text">{{ project.description }}</p></div>
        </div>
      </a>
    </div>
  {% endfor %}
</div>
