---
layout: page
title: Friends
permalink: /friends/

excerpt: Real and virtual people. All together.
---


# In no particular order and with no reason at all, I simply like to read or see what they're doing and they all inspire me in some way. The resurgence of the personal site starts with microinteractions! If you have a couple minutes, take a look at:


<ul class="category friends small">
{% for friend in site.data.friends %}
  <a href="https://{{ friend.website }}" target="_blank">
    <li>
        <span class="title">{{ friend.name }}</span>
        <span class="description">{{ friend.website }}</span>
    </li>
  </a>
{% endfor %}
</ul>