---
layout: index
title: Home
menu_title: Home /
feature_text: |
  Selen Apaydın
feature_subtext: |
  
feature_image: /assets/img/piano010-pianoles-rotterdam.jpg
excerpt: |
  Selen A.
lang: en
page_id: home
permalink: /
---

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