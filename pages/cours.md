---
layout: page
title: Cours disponibles
permalink: /cours.html
---

{% for cours in site.cours %}

<a href="{{ cours.url | prepend: site.baseurl }}">
  <h2>{{ cours.title }}</h2>
</a>

<p class="post-excerpt">{{ cours.description | truncate: 160 }}</p>
cours.level
cours.examen

{% endfor %}  
