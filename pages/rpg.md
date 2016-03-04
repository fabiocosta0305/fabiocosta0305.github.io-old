---
layout: page
show_meta: false
subheadline: "RPG"
title: "Meus Materiais de RPG!"
teaser: "Esses são alguns materiais de RPG que tenho aqui nos meus cacarecos. Fique a vontade para se Servir"
permalink: "/rpg/"
---

<h1>Meus Materias de Fate</h1>

<ul>
    {% for post in site.tags.fate %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
