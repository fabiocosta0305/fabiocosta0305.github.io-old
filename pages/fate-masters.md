---
layout: page
show_meta: false
subheadline: "Fate"
title: "Fate Masters"
teaser: "O Podcast dos Algozes dos Jogadores!"
header:
    image_fullwidth: FundoBlog.png
permalink: "/fate-masters/"
---

Esse é  o podcast onden você  irá aprender a  fazer tudo o que  um bom
Mestre precisa fazer: roubar, trapacear, sacanear, enganar, acabar com
a  felicidade dos  seus jogadores  e, acima  de tudo,  tornar aventura
épica  e divertida  para você  e seus  jogadores. Aqui  colocaremos os
materiais e os áudios do Podcast do Fate Masters.

- [Assine o _feed_ do Fate Masters em MP3][fate-masters-feed]
- [Assine o _feed_ do Fate Masters em Ogg Vorbis][fate-masters-ogg-feed]

<ul>
    {% for post in site.tags.fate-masters %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

[fate-masters-feed]: <http://feeds.feedburner.com/FateMastersRPG>
[fate-masters-ogg-feed]: <http://feeds.feedburner.com/FateMastersRPG-OGG>
