---
layout:     page
title:      Bookmarks
permalink:  /bookmarks/
excerpt:    The neverending archive
---


<ul class="category">
{% for link in site.data.bookmarks %}
  <a href="https://{{ link.website }}" target="_blank">
    <li>
        <span class="number">No.{{ link.number }}</span>
        <span class="title">{{ link.name }}</span>
        <span class="info2">{{ link.date | date_to_string }}</span>
        <span class="info">{{ link.description }}</span>
    </li>
  </a>
{% endfor %}
</ul>