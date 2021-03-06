---
title: "Le temps liturgique"
layout: page
# title:  "Le Temps Liturgique pour découvrir ou méditer la Bible par petit morceaux cohérents"
permalink: /temps_liturgique/
---

## Le Temps Liturgique pour découvrir ou méditer la Bible par petit morceaux cohérents

![right 50]({{site.baseurl}}images/bigben.jpg)

L'Eglise catholique a placé chaque jour dans un temps liturgique.
Et elle propose une messe différente pour chaque jour.
Avec 3 textes bibliques (4 le dimanche) :
- une "première lecture"
- un psaume (ou parfois un cantique biblique)
- une "deuxième lecture" (le dimanche et aux grandes fêtes)
- un évangile.

Ces textes sont donnés ensemble parce qu'ils s'éclairent mutuellement.

Les grandes périodes du temps liturgique sont:
- l'Avent
- le temps de Noël
- le temps "ordinaire"
- le Carême
- le temps de Pâques
- le temps ordinaire (qui reprend là où il s'était arrêté).

Les mêmes textes du temps ordinaire reviennent tous les 2 ans pour la semaine (on distingue les années paires et impaires).
Et tous les 3 ans pour les dimanches (on distingue les années A, B, C).
Les textes ne changent pas d'une année à l'autre pour les autres périodes du temps liturgique,
ni pour les messes de fêtes ou en l'honneur des saints.

On choisit les textes qu'on veut pour les messes de mariage, de profession solennelle ou d'obsèques.

### Accès par temps liturgique

{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}

{% assign cats = site.categories | sort %}

{% for category in cats %}
  <h4>{{ category[0] }}</h4>
  <ul>
    {% for post in category[1] %}
    <li>
      <a  href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>
      <span class="post-meta">({{ post.date | date: date_format }})</span>
    </li>
    {% endfor %}
  </ul>
{% endfor %}
