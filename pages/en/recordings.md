---
layout: page
title: Recordings
menu_title: Recordings /
feature_text: |
  Recordings
feature_subtext: |
  Recordings
feature_image: /assets/img/piano010-pianoles-rotterdam.jpg
excerpt: |
  Recordings
lang: en
page_id: recordings
permalink: /recordings
carousels:
  - videos: 
    - id: mv1asI5RHVI
    - id: -2bCphYIE-A
    - id: KhYqdfXLuog
    - id: IyAyr91JiV0
    - id: z6OgpYP3pjM
    - id: XvtvJiXdI0w
---

<section id="wide-div">
  <div id="carousel">
    {% for item in page.carousels[0].videos %}
      <div>
        {% include video.html id=item.id %}
      </div>
    {% endfor %}
  </div>
</section>

## Other performance recordings
<br>
  {% for item in site.data.lists.recordings %}
#### {{ item.title }}
{{ item.subtitle }}
  {% endfor %}