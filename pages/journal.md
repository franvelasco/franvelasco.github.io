---
layout: page
title: Journal
permalink: /journal/
excerpt: Improving my writing skills, word by word.
---

<ul class="category">
{% for category in site.categories reversed %}
  <h1><a class="{{ category | first }}" name="{{ category | first }}" id="#{{ page.categories }}">On {{ category | first }}</a></h1>
    <ul class="category">
    {% for post in category.last %}
      <li class="category-post">
      	<a href="{{ post.url }}">{{ post.title }} <span class="category-post-date">{{ post.date | date_to_string }}</span></a>
      </li>
    {% endfor %}
    </ul><br><br><br>
{% endfor %}
</ul>