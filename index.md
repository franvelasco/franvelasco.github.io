---
layout: page
title: Another personal site.

excerpt: Welcome to mine.
info-cat:
info-date: 
info-place: 
---

<span class="big-text">
Hello, my name is *Fran Velasco*. I live in Madrid with my wife *Cecilia*, my kids *Max* & *Oli*, and a cat named *Petra*. I like to travel as much as possible, I design things in *Seabell Studio*, I take my *camera* everywhere, I play *bass guitar*, I love/hate social networks, I collect *Marvel* books and *Hot Wheels*, and I'd eat *pizza* every day.
</span>

<br>

<div class="gallery-post" markdown="1">

![This is Fran Velasco. April 2020](../assets/imgs/fran-profile.jpg)

<div>

<h1>Latest Post</h1>
{% for post in site.posts limit:1 %}
... Show the first post all big ...
{% endfor %}
<h1>Recent Posts</h1>
{% for post in site.posts offset:1 limit:2 %}
... Show the next two posts ...
{% endfor %}