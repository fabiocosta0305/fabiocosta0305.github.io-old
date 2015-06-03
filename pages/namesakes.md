---
layout: page
show_meta: false
subheadline: "Namesakes"
title: "Meus Materiais de Namesakes!"
teaser: "Esses são alguns materiais de Namesakes que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/fate-core/namesakes/"
---
<ul>
    {% for post in site.tags.Namesakes %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
