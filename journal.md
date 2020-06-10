---
layout: page
title: Journal
permalink: /journal/
excerpt: Improving my writing skills, word by word.
---

<ul class="categorias">
{% for category in site.categories %}
  <li><h1><a class="{{ category | first }}" name="{{ category | first }}">{{ category | first }}</a></h1>
    <ul class="categorias">
    {% for post in category.last %}
      <li class="categoria-post"><a href="{{ post.url }}">{{ post.title }} <span class="categoria-post-date">{{ post.date | date: "%Y" }}</span></a></li>
    {% endfor %}
    </ul><br><br><br>
  </li>
{% endfor %}
</ul>