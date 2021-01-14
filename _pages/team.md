---
title: "Brain AI Lab - Team"
layout: gridlay
excerpt: "BrainAI Lab: Team members"
sitemap: false
permalink: /team/
---

# Team

- If you're interested in joining our team, please email Sangtae Ahn (<stahn@knu.ac.kr>)

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-xs-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br>
  <i>email: <{{ member.email }}></i>
  
  {% if member.number_educ == 1 %}
  {{ member.education1 }}
  {% endif %}
<br>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Alumni
#### Undergraduate Research Assistants  
Hyeon Su Kwon, Young Hoon Park, Hyun Ji Gwon, Eun Chan Lee, Hyun Jin Jang


