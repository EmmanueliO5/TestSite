---
layout: default
title: Now
---

<ul class="ledger">
{% for post in site.posts %}
  <li class="ledger-item">
    <span class="ledger-date">{{ post.date | date: "%Y·%m·%d" }}</span>
    <div>
      <h3 class="ledger-title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
    </div>
  </li>
{% endfor %}
</ul>