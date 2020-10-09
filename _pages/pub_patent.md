---
title: "BrainAI Lab - Publications - Patents"
layout: textlay
excerpt: "BrainAI Lab -- Publications - Patents."
sitemap: false
permalink: /pub_patent/
---


# Publications

see also [Google Scholar](https://scholar.google.com/citations?hl=en&user=F-LXQwcAAAAJ&view_op=list_works&sortby=pubdate)

## Patents

{% for publi in site.data.publist_patent %}

  {{ publi.title }} <br />
  {{ publi.authors }} <br />
  <em>{{ publi.journal }}</em> <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}


