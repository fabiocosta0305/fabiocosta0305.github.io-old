---
layout: page
show_meta: false
title: "Personagens exemplos"
permalink: "/personagens/"
---

    
Alguns personagens exemplos que eu criei

<ul> 
  {% assign tag = "" %}
  {% assign first = "" %}
  {% for post in site.categories.personagens %}
  {% if post.tags != tag %}
  {% if first != "" %}
  </ul>
  {% endif %}
  {% assign tag = post.tags %}    
  {% assign first = "blah" %}
   <li><h3> {{ post.tags }} </h3></li>
  <ul>
  {% endif %}
   <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }} </a> </li>
    {% endfor %}
  </ul>
</ul>

Some characters I did (in English)

<ul> 
  {% assign tag = "" %}
  {% assign first = "" %}
  {% for post in site.categories.characters %}
  {% if post.tags != tag %}
  {% if first != "" %}
  </ul>
  {% endif %}
  {% assign tag = post.tags %}    
  {% assign first = "blah" %}
   <li><h3> {{ post.tags }} </h3></li>
  <ul>
  {% endif %}
   <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }} </a> </li>
    {% endfor %}
  </ul>
</ul>
