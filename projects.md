---
layout: default
title: Projects
permalink: /projects/
---

# Projects

A collection of my work and experiments.

<div class="projects-grid">
{% for project in site.projects %}
<div class="project-card">
  <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
  <p>{{ project.description }}</p>
  {% if project.tags %}
  <div class="project-tags">
    {% for tag in project.tags %}
    <span class="tag">{{ tag }}</span>
    {% endfor %}
  </div>
  {% endif %}
</div>
{% endfor %}
</div>
