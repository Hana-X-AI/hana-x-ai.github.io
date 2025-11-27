---
layout: default
title: Articles
permalink: /articles/
---

# Articles

Thoughts, tutorials, and insights.

<div class="articles-list">
{% for post in site.posts %}
<article class="article-card">
  <header>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
  </header>
  {% if post.excerpt %}
  <p class="article-excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
  {% endif %}
  {% if post.tags %}
  <div class="post-tags">
    {% for tag in post.tags %}
    <span class="tag">{{ tag }}</span>
    {% endfor %}
  </div>
  {% endif %}
</article>
{% endfor %}
</div>

{% if site.posts.size == 0 %}
<p class="no-articles">No articles yet. Check back soon!</p>
{% endif %}
