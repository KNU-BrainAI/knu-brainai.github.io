---
title: "Brain AI Lab - Publications"
layout: textlay
excerpt: "BrainAI Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

see also [Google Scholar](https://scholar.google.com/citations?hl=en&user=F-LXQwcAAAAJ&view_op=list_works&sortby=pubdate)

### Journals & Conferences

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: center" />
  {{ publi.authors }} <br />
  <em>{{ publi.journal }}</em> <a href="{{ publi.link.url }}">{{ publi.link.display }}</a><br />
   </div>
</div>
  

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}


<!---

COMMENT

{% for publi in site.data.publist_conf %}

  {{ publi.title }} <br />
  {{ publi.authors }} <br />
  <em>{{ publi.journal }}</em> <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

-->

### Patents

{% for publi in site.data.publist_patent %}

  {{ publi.title }} <br />
  {{ publi.authors }} <br />
  <em>{{ publi.journal }}</em> <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
