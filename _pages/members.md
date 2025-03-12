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

  {% if member.number_educ == 4 %}
  {{ member.education1 }}<br>
  {{ member.education2 }}<br>
  {{ member.education3 }}<br>
  {{ member.education4 }}
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
#### Master Students
2025.02 이지훈 PhD Student @ KNU Graduate School <br>
2025.02 배찬호 Researcher @ AI Robotics <br>
2024.08 차도흔 PhD Student @ KNU Graduate School <br>
2024.02 이승훈 Researcher @ Hanhwa Systems <br>
2023.02 김예림 Researcher @ DGIST <br>
2023.02 이은찬 PhD Student @ UNIST <br>

#### Undergraduate Researchers  
2024.12 양재모 Samsung Electronics<br>
2024.12 김민석 Samsung Electronics<br>
2024.12 편수빈 Samsung Electronics<br>
2024.12 박성국 Hyundai Mobis<br>
2024.12 박영은 Hanhwa Systems<br>
2024.12 민윤홍 KAIST Graduate School<br>
2024.08 김휘동 KAIST Graduate School<br>
2024.02 진채영 KAIST Graduate School<br>
2024.02 전승빈 KNU Graduate School<br>
2024.02 전수형 LG Electronics<br>
2024.02 박진수 Hyundai Motor Company<br>
2024.02 이희원 Yonsei Univ. Graduate School<br>
2023.02 이동엽 POSTECH Graduate School<br>
2022.08 차도흔 KNU Graduate School<br>
2022.02 장현진 KNU Graduate School<br>
2022.02 이승훈 KNU Graduate School<br>
2022.02 박재성 KAIST Graduate School<br>
2022.02 이창현 UNIST Graduate School<br>
2021.08 박시은 KNU Graduate School<br>
2021.06 권현수 LG Electronics <br>
2021.02 이은찬 KNU Graduate School<br>
