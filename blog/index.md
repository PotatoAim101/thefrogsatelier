---
layout: default
title: Blog
---

<h1>Blog</h1>
<p>All my knitting thoughts, sorted from newest to oldest.</p>

<ul class="item-list">
  {% for post in site.posts %}
    <li>
      <span class="item-date">{{ post.date | date: "%B %-d, %Y" }}</span>
      <h2>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>