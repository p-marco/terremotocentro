---
layout: page
title: Vittime
description: Questa pagina raccoglie l'elenco delle vittime del terremoto che il 24 agosto 2016 ha colpito il centro Italia.
permalink: /vittime/
---

Cognome         |Nome                    |Prefettura   |Data di nascita|Luogo di nascita    |Fonte
:---------------|:-----------------------|:------------|:--------------|:-------------------|:----------------------------------------------------------------
{% for member in site.data.vittime %} {{member.Cognome}} | {{member.Nome}} | {{member.Prefettura}} | {{member.Data}} | {{member.Luogo}} | [Fonte]({{member.Fonte}})
{% endfor %}


<div class="posts">
  {% for post in site.posts %}
    {% if post.categories contains 'vittime' %}
      <article class="post">
        <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

        <div class="entry">
          {{ post.excerpt }}
        </div>

        <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Leggi Tutto</a>
      </article>
    {% endif %}
  {% endfor %}
</div>

