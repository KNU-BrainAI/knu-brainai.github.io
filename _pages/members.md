---
title: "Brain AI Lab - Members"
layout: gridlay
excerpt: "Brain AI Lab : Members"
sitemap: false
permalink: /members/
---

# Members

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
  
  <h5>{{ member.interest }}</h5>
  
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
#### Masters Students
2024.02 이승훈 한화시스템 <br>
2023.02 김예림 Researcher, DGIST <br>
2023.02 이은찬 PhD Student, UNIST <br>

#### Undergraduate Researchers  
2024.02 박진수 현대자동차<br>
2023.02 이동엽 POSTECH Graduate School<br>
2022.08 차도흔 KNU Graduate School<br>
2022.02 장현진 KNU Graduate School<br>
2022.02 이승훈 KNU Graduate School<br>
2022.02 박재성 KAIST Graduate School<br>
2021.12 이창현 UNIST Graduate School<br>
2021.08 박시은 KNU Graduate School<br>
2021.06 권현수 LG전자 <br>
2021.02 이은찬 KNU Graduate School<br>
2020.12 권현지 한국항공우주<br>
