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

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <h5>{{ member.info }}<br></h5>
  <i>email: <{{ member.email }}></i>
  
  {% if member.number_educ == 1 %}
  {{ member.education1 }}
  {% endif %}
  
  {% if member.number_educ == 2 %}
  {{ member.education1 }}<br>
  {{ member.education2 }}
  {% endif %}
  
  {% if member.number_educ == 3 %}
  {{ member.education1 }}<br>
  {{ member.education2 }}<br>
  {{ member.education3 }}
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
#### Undergraduate Researchers  
(Spring, 2021) 박시은 <br>
(Fall, 2020) 권현수, 권현지, 박영훈, 이은찬, 장현진
