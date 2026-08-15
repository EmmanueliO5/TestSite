---
layout: posts
title: What Have I Done??
---

<ul>
{% for project in site.projects %}
  <li>
    <a href="{{ project.url }}">{{ project.title }}</a> — {{ project.summary }}
  </li>
{% endfor %}
</ul>