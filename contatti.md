---
layout: page
title: Fonti
description: Questa pagina contiene l'elenco dei contatti delle Associazioni e degli Enti impiegati nelle operazioni di assistenza alla popolazione terremotata.
permalink: /fonti/
---
{% for member in site.data.contatti %}
  <div class="row">
  <div class="col-md-2">
{{member.Nome}}
</div>
  <div class="col-md-2">
{{member.Numero}}
</div>
</div>
{% endfor %}
