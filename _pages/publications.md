---
title: "BrainAI Lab - Publications"
layout: textlay
excerpt: "BrainAI Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Journals

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
