---
layout: page
show_meta: false
subheadline: "Destino de Moreania"
title: "O Destino de Moreania"
teaser: "Minha Adaptação para Fate Core de Reinos de Moreania, o cenário oficial da DragonSlayer"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/moreania/"
---
<ul>
{% for post in site.tags.moreania %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
