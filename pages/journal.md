---
layout: page
title: Journal
permalink: /journal/
excerpt: Improving my writing skills, word by word.
---


<ul>
{% for category in site.categories %}
  <li><h1><a class="journal {{ category | first }}" name="{{ category | first }}" id="#{{ page.categories }}">● </a>{{ category | first }}</h1>
    <ul class="category">
    {% for post in category.last %}
      <a href="{{ post.url }}"><li>
        <span class="number">No. {{ post.number }}</span><span class="title">{{ post.title }}</span><span class="info">{{ post.date | date_to_string }}</span>
      </li></a>
    {% endfor %}
    </ul><br><br><br><br><br>
  </li>
{% endfor %}
</ul>