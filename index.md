---
layout: default
title: Inicio
---

# Bienvenido a *Mi Blog* 👋

Este es un blog construido con **Jekyll** y un tema oscuro personalizado.  
Incluye tres entradas de ejemplo, un diseño limpio y navegación clara.

{% for post in site.posts %}
---
### [{{ post.title }}]({{ post.url }})
*Publicado el {{ post.date | date: "%d/%m/%Y" }}*  
{{ post.excerpt }}
{% endfor %}
