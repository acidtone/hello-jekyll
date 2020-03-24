---
layout: default
title: RPG Character Archetypes
description: 
---
# {{page.title}}
<section>
  {% for character in site.characters %}
  <article>
    <h2>{{character.name}}</h2>
    <p>Specialty: {{character.specialty}}</p>
    {{ character.content | markdownify}}
    <p><a href="{{character.source}}">Source</a></p>
  </article>
  {% endfor %}
</section>
