---
layout: page
show_meta: false
subheadline: "Fate"
title: "Meus Materiais de Fate!"
teaser: "Esses são alguns materiais de Fate que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/fate/"
---
<ul>
    {% for post in site.tags.fate %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
