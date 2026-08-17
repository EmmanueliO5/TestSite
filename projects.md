---
layout: default
title: Projects
---

<ul class="ledger">
{% for project in site.projects %}
  <li class="ledger-item">
    <span class="ledger-date">{{ project.date | default: "" | date: "%Y·%m" }}</span>
    <div>
      <h3 class="ledger-title"><a href="{{ project.url }}">{{ project.title }}</a></h3>
      <p class="ledger-summary">{{ project.summary }}</p>
      <span class="ledger-tags">{{ project.stack }}</span>
    </div>
  </li>
{% endfor %}
</ul>