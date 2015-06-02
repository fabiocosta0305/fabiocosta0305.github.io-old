---
layout: page
show_meta: false
subheadline: "Fate Core"
title: "Meus Materiais de Fate Core!"
teaser: "Esses são alguns materiais de Fate Core que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/fate-core/"
---
<ul>
    {% for post in site.tags.fate_core %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

<ul>
    {% for tag in site.tags %}
    <li>{{ tag.title }}</li>
    {% endfor %}
</ul>