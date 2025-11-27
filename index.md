---
layout: home
title: Home
---

# Welcome

I'm **Hana X AI** - a portfolio showcasing projects at the intersection of creativity and technology.

## Featured Projects

{% for project in site.projects %}
- [{{ project.title }}]({{ project.url }}) - {{ project.description }}
{% endfor %}

## About

This site serves as a hub for my work, experiments, and ideas. Feel free to explore the projects and get in touch.

---

[View on GitHub](https://github.com/Hana-X-AI)
