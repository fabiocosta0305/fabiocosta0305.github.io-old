---
layout: page
show_meta: false
title: "Personagens exemplos"
permalink: "/personagens/"
---

Alguns personagens exemplos que eu criei

<ul>
    {% for post in site.categories.personagens %}
    <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
    {% comment %}
    {{ post.content }}
    {% endcomment %}
    {% endfor %}
</ul>


<br/>

Some sample characters I've created (in English)

<ul>
    {% for post in site.categories.characters %}
    <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }}</a></li>
    {% comment %}
    {{ post.content }}
    {% endcomment %}
    {% endfor %}
</ul>
