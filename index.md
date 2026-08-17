---
layout: default
title: Home
---

<div class="hero">
  <h1>Hi, I'm Emmanuel — I Like Building Robots.</h1>
  <p>This is a running record of projects I've worked on and what I'm doing right now!</p>
  <div class="status-line">
    <span class="status-dot"></span>
    Currently building: This Website!
  </div>
</div>

<h2 style="font-size:14px; font-family:'IBM Plex Mono',monospace; text-transform:uppercase; color:var(--graphite); letter-spacing:0.03em;">Recent</h2>

<ul class="ledger">
{% for project in site.projects limit:3 %}
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