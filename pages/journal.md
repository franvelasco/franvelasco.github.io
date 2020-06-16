---
layout: page
title: Journal
permalink: /journal/
excerpt: Improving my writing skills, word by word.
---

<ul>
{% for category in site.categories reversed %}
  <li><h1><a class="{{ category | first }}" name="{{ category | first }}" id="#{{ page.categories }}">{{ category | first }}</a></h1>
    <ul class="category">
    {% for post in category.last %}
      <li><a href="{{ post.url }}">{{ post.title }} <span class="date">{{ post.date | date_to_string }}</span></a></li>
    {% endfor %}
    </ul><br><br><br><br><br>
  </li>
{% endfor %}
</ul>