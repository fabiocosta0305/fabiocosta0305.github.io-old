---
layout: page
show_meta: false
subheadline: "Destino da Caduceus"
title: "O Destino da Caduceus"
teaser: "Minha Adaptação para Fate Core de Reinos de Moreania, o cenário oficial da DragonSlayer"
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-core/caduceus/"
---
<ul>
    {% for post in site.tags.Destino-da-Caduceus %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
