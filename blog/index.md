---
title: 新闻
nav:
  order: 3
  tooltip: 实验室活动和新闻展示
---

# {% include icon.html icon="fa-solid fa-feather-pointed" %}新闻



{% include section.html %}

{% include search-box.html %}

{% include tags.html tags=site.tags %}

{% include search-info.html %}

## Conferences

{% include list.html component="card" data="tools" filters="group: conference"%}

{% include section.html %}

## Reports

{% include list.html component="card" data="tools" filters="group: report"%}

{% include section.html %}

## Contact

地址：中国上海曹安公路4800号同济大学软件学院 <br>
邮编：201804 <br>
联系电话：86-21-69589585, 69589332(FAX)

{%
  include button.html
  type="email"
  text="email"
%}

{%
  include button.html
  type="address"
  text="address"
%}

{% capture col1 %}

{%
  include figure.html
  image="images/sse.png"
  caption="同济大学软件学院"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/tongji.png"
  caption="同济大学"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}
