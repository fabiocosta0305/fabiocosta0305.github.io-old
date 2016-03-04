---
layout: page
show_meta: false
title: "Meus Materiais de RPG"
permalink: "/rpg/"
---

Materias de RPG que Escrevi com o tempo

<ul>
    {% for post in site.tipos %}
    <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
    {% comment %}
    {{ post.content }}
    {% endcomment %}
    {% endfor %}
</ul>

