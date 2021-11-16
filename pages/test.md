---
layout:     page
title:      The Playground
permalink:  /z
excerpt:    Welcome to The Lab
---


###### <a class="lang-selector" onclick="openLang('eng')">ENGLISH</a> — <a class="lang-selector"  onclick="openLang('esp')">ESPAÑOL</a>

<script>
function openLang(langName) {
  var i;
  var x = document.getElementsByClassName("lang");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  document.getElementById(langName).style.display = "block";  
}
</script>

<div id="eng" class="lang">

Hello, my name is Fran Velasco. I live in Madrid with my wife Cecilia, my kids Max & Oli, and a cat named Petra. I like to travel as much as possible, I design things in Seabell Studio, I take my camera everywhere, I play bass guitar, I love/hate social networks, I collect Marvel books and Hot Wheels, and I’d eat pizza every day.

<div class="gallery-{{ page.layout }}" markdown="1">

![](https://franvelas.co/assets/imgs/fran-profile.jpg)

</div>

I design things in Seabell Studio

</div>



<div id="esp" class="lang" style="display:none">

Hola, mi nombre es Fran Velasco. Vivo en Madrid con mi esposa Cecilia, mis hijos Max & Oli y una gata llamada Petra. Me gusta viajar tanto como sea posible, diseño cosas en Seabell Studio, llevo mi cámara a todas partes, toco el bajo, amo / odio las redes sociales, colecciono libros de Marvel y Hot Wheels, y comía pizza todos los días.

<div class="gallery-{{ page.layout }}" markdown="1">

![](https://franvelas.co/assets/imgs/fran-profile.jpg)

</div>

Diseño cosas en Seabell Studio

</div>




<br><br><br><br><br><br><br><br><br><br>

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