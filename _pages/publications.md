---
title: "BrainAI Lab - Publications"
layout: textlay
excerpt: "BrainAI Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

see also [Google Scholar](https://scholar.google.com/citations?hl=en&user=F-LXQwcAAAAJ&view_op=list_works&sortby=pubdate)

## Journals

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  {{ publi.authors }} <br />
  <em>{{ publi.journal }}</em> <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

## Conferences
