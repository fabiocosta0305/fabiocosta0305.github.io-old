---
layout: page
show_meta: false
title: "Personagens exemplos"
permalink: "/personagens/"
---

    
Alguns personagens exemplos que eu criei

{% capture site_tags %}{% for post in site.categories.personagens %}{% for tag in post.tags %}{{ tag | lstrip | rstrip }},{% endfor %}{% endfor %}
{% endcapture %}

<!-- `tag_words` is a sorted array of the tag names. -->
{% assign tag_words = site_tags | strip_newlines | strip | split:',' | sort %}
{% assign tags = tag_words[1] %}


{% for item in tag_words %}
    {% unless tags contains item %}
        {% capture tags %}{{ tags }}|{{ item }}{% endcapture %}
    {% endunless %}
{% endfor %}

{% assign taglist = tags | strip_newlines | strip | split:'|' | sort %}

<ul> 
{% for tag in taglist %}
   <li><h3> {{ tag }} </h3></li>
   <ul>
   {% for post in site.categories.personagens %}
   {% if post.tags contains tag %}
   <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }} </a> </li>
   {% endif %}
   {% endfor %}
   </ul>
{% endfor %}
</ul>

{% comment %}
<ul> 
  {% assign tag = "" %}
  {% assign first = "" %}
  {% for post in site.categories.personagens %}
  {% if post.tags != tag %}
  {% if first != "" %}
  </ul>
  {% endif %}
  {% assign tag = post.tags %}    
  {% assign first = "blah" %}
   <li><h3> {{ post.tags }} </h3></li>
  <ul>
  {% endif %}
   <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }} </a> </li>
    {% endfor %}
  </ul>
</ul>
{% endcomment %}

Some characters I did (in English)

{% capture site_tags %}{% for post in site.categories.characters %}{% for tag in post.tags %}{{ tag | lstrip | rstrip }},{% endfor %}{% endfor %}
{% endcapture %}

<!-- `tag_words` is a sorted array of the tag names. -->
{% assign tag_words = site_tags | strip_newlines | strip | split:',' | sort %}
{% assign tags = tag_words[1] %}


{% for item in tag_words %}
    {% unless tags contains item %}
        {% capture tags %}{{ tags }}|{{ item }}{% endcapture %}
    {% endunless %}
{% endfor %}

{% assign taglist = tags | strip_newlines | strip | split:'|' | sort %}

<ul> 
{% for tag in taglist %}
   <li><h3> {{ tag }} </h3></li>
   <ul>
   {% for post in site.categories.characters %}
   {% if post.tags contains tag %}
   <li><a href="{{ post.url }}">{{ post.title | markdownify | remove: '<p>' | remove: '</p>' }} </a> </li>
   {% endif %}
   {% endfor %}
   </ul>
{% endfor %}
</ul>


{% comment %}

Apenas para referência de código

{% capture site_tags %}{% for post in site.categories.personagens %}{% for tag in post.tags %}{{ tag }},{% endfor %}{% endfor %}
{% endcapture %}

<!-- `tag_words` is a sorted array of the tag names. -->
{% assign tag_words = site_tags | split:',' | sort %}
{% assign tags = tag_words[1] %}

{% for item in tag_words %}
    {% unless tags contains item %}
        {% capture tags %}{{ tags }}|{{ item }}{% endcapture %}
    {% endunless %}
{% endfor %}

{{ tag_words }} 

{{ tags }}

{% endcomment %}
