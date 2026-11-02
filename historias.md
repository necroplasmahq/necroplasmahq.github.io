---
layout: default
title: Histórias
description: Arcos, edições e publicações do universo Spawn.
permalink: /historias/
---

<div class="catalog-intro">
  <h1>Histórias</h1>
  <p>Explore os arcos narrativos, edições originais e publicações do universo Spawn.</p>

  <section id="arcos" class="catalog-group">
    <h2>Arcos</h2>

    {% if site.arcos.size > 0 %}
      <ul>
        {% for arco in site.arcos %}
          <li>
            <a href="{{ arco.url | relative_url }}">
              {{ arco.title | escape }}
            </a>
          </li>
        {% endfor %}
      </ul>
    {% else %}
      <p>Nenhum arco cadastrado.</p>
    {% endif %}
  </section>

  <section id="edicoes" class="catalog-group">
    <h2>Edições</h2>

    {% if site.edicoes.size > 0 %}
      <ul>
        {% for edicao in site.edicoes %}
          <li>
            <a href="{{ edicao.url | relative_url }}">
              {{ edicao.title | escape }}
            </a>
          </li>
        {% endfor %}
      </ul>
    {% else %}
      <p>Nenhuma edição cadastrada.</p>
    {% endif %}
  </section>

  <section id="publicacoes" class="catalog-group">
    <h2>Publicações</h2>

    {% if site.publicacoes.size > 0 %}
      <ul>
        {% for publicacao in site.publicacoes %}
          <li>
            <a href="{{ publicacao.url | relative_url }}">
              {{ publicacao.title | escape }}
            </a>
          </li>
        {% endfor %}
      </ul>
    {% else %}
      <p>Nenhuma publicação cadastrada.</p>
    {% endif %}
  </section>
</div>
