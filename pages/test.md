---
layout:     page
title:      New Stuff
permalink:  /z
excerpt:    Probando, probando!
---


<div class="w3-container">
  <h2>Tabs</h2>
  <p>Tabs are perfect for single page web applications, or for web pages capable of displaying different subjects. Click on the links below.</p>
</div>

<div class="w3-bar w3-black">
  <button class="w3-bar-item w3-button" onclick="openCity('London')">London</button>
  <button class="w3-bar-item w3-button" onclick="openCity('Paris')">Paris</button>
  <button class="w3-bar-item w3-button" onclick="openCity('Tokyo')">Tokyo</button>
</div>

<div id="London" class="w3-container city">
  <h2>London</h2>
  <p>London is the capital city of England.</p>
</div>

<div id="Paris" class="w3-container city" style="display:none">
  <h2>Paris</h2>
  <p>Paris is the capital of France.</p> 
</div>

<div id="Tokyo" class="w3-container city" style="display:none">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
</div>

<script>
function openCity(cityName) {
  var i;
  var x = document.getElementsByClassName("city");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  document.getElementById(cityName).style.display = "block";  
}
</script>

---

# Everything I've written, ever.

<ul class="category">
	{% for post in site.posts %}	
      <a href="{{ post.url }}"><li>
        <span class="number">No. {{ post.number }}</span>
        <span class="title">{{ post.title }}</span>
        <span class="date">{{ post.date | date_to_string }}</span>
      </li></a>
	{% endfor %}
</ul>


---

<span class="big-text">This is huge, big-text</span>

# This is an H1 header

## This is an H2 header

### This is an H3 header

#### This is an H4 header

##### This is an H5 header

###### This is an H6 header

---

This is body text

---

{% include search-lunr.html %}

---

{% include instagram.html username="franvelas.co" %}