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
  {{ publi.authors }} <br />
  <em>{{ publi.journal }}</em> <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
