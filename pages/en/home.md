---
layout: index
title: Home
menu_title: Home /
feature_text: |
  Selen Apaydın
feature_subtext: |
  Selen Apaydın is a concert pianist whose stage presence in combination with her mastery of the keyboard and sensitivity expressed through the manipulation of sound made her name recognized. 
feature_image: /assets/img/piano010-pianoles-rotterdam.jpg
excerpt: |
  Selen A.
lang: en
page_id: home
permalink: /
---

<h1 style='display: none;'>Home | Selen Apaydın</h1>
## News

  {% for item in site.data.lists.news %}
#### {{ item.title }}
{{ item.subtitle }}
  {% endfor %}

## Events

  {% for item in site.data.lists.events %}
#### {{ item.date }}
{% if item.project %}##### {{ item.project }} <br>{% endif %}
{{ item.title }} <br>
<small>{{ item.description }}</small>
  {% endfor %}