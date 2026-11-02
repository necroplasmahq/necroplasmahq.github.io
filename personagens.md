---
layout: default
title: Personagens
description: Personagens, relações e aparições do universo Spawn.
permalink: /personagens/
---

<section class="catalog-intro">
  <h1>Personagens</h1>
  <p>Conheça os personagens e suas relações no universo Spawn.</p>

  {% assign personagens = site.personagens | sort: "title" %}

  {% if personagens.size > 0 %}
    <ul>
      {% for personagem in personagens %}
        <li>
          <a href="{{ personagem.url | relative_url }}">
            {{ personagem.title | escape }}
          </a>
        </li>
      {% endfor %}
    </ul>
  {% else %}
    <p>Nenhum personagem cadastrado.</p>
  {% endif %}
</section>
