---
---

{% include section.html %}

## 新闻


{% capture text %}

这里是第一条新闻。

{%
  include button.html
  link="news"
  text="查看第一条新闻"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="news"
  title="新闻"
  text=text
%}