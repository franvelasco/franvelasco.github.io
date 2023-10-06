---
layout: page
title: Journal
permalink: /journal/
excerpt: Improving my writing skills, word by word.
---

<ul class="categorias">
{% for category in site.categories reversed %}
  <li><h1><a class="{{ category | first }}" name="{{ category | first }}" id="#{{ page.categories }}">{{ category | first }}</a></h1>
    <ul class="categorias">
    {% for post in category.last %}
      <li class="categoria-post"><a href="{{ post.url }}">{{ post.title }} <span class="categoria-post-date">{{ post.date | date_to_string }}</span></a></li>
    {% endfor %}
    </ul><br><br><br>
  </li>
{% endfor %}
</ul>