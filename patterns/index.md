---
layout: default
title: Knitting Patterns
---

<h1>Knitting Patterns</h1>
<p>My collection of knitting patterns. I hope you enjoy them!</p>

<ul class="item-list">
  {% for pattern in site.patterns reversed %}
    <li>
      <h2>
        <a href="{{ pattern.url }}">{{ pattern.title }}</a>
      </h2>
      {% if pattern.summary %}
        <p>{{ pattern.summary }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% if site.patterns.size == 0 %}
  <p>No patterns just yet, but I'm working on some! Check back soon. 🐸</p>
{% endif %}