---
layout: default
title: Início
---

# Bem-vindo ao Necroplasma

Um espaço independente dedicado ao universo Spawn, seus quadrinhos, personagens, histórias e publicações.

Aqui você encontra registros, curiosidades, resenhas e textos pessoais sobre o personagem criado por Todd McFarlane.

## Últimas publicações

{% for post in site.posts limit:5 %}
### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | strip_html | truncatewords: 35 }}

{% endfor %}
