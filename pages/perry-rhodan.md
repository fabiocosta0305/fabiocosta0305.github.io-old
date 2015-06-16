---
layout: page
show_meta: false
subheadline: "Fate Core"
title: "Meus Materiais do Destino de Perry Rhodan!"
teaser: "Esses são alguns materiais do Destino de Perry Rhodan que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-core/perry-rhodan/"
---
<ul>
    {% for post in site.tags.Perry-Rhodan %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

