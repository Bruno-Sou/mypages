---
layout: page
title:  "La Bible"
date:   2018-06-06
permalink: /bible/
---

Les textes sont présentés dans la traduction de la liturgie catholique (cf. [aelf.org]
). J'ai mis des sauts de page là où j'ai envie de respirer quand je lis à haute voix
et des majuscule quand l'auteur biblique parle de Dieu ou s'adresse à Lui, car cela m'aide à penser qu'on parle à Dieu ou de Lui.

En PJ, on trouvera la dernière méditation qu'il m'a été donné de faire dans la journée,
avec les homélies et commentaires bibliques que j'ai pu avoir ce jour là.

Les encadrés rouge expriment ce que j'ai compris d'un verset qui me fait particulièrement réfléchir.
Ils n'engagent que moi ; ils sont là pour pousser le lecteur de la Bible à faire de même pour faire entrer en lui la Parole.

J'invite le lecteur qui veut en savoir plus sur l'interprétation habituelle donnée à un verset
à consulter une Bible et ses notes, voir plusieurs Bibles s'il veut creuser.

Ce site est construit à l'aide de GitHub et du langage d'édition Jekyll.


### Accès par référence biblique

{% assign tags = site.tags | sort %}
{% for tag in tags %}
  <h4>{{ tag[0] }}</h4>
  <ul>
    {% for post in tag[1] %}
    <li>
      <a  href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>
      <span class="post-meta">({{ post.date | date: date_format }})</span>
    </li>
    {% endfor %}
  </ul>
{% endfor %}


[aelf.org]: https://www.aelf.org
