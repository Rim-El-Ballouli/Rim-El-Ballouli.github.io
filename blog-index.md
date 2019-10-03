---
layout: default
title: Rim El Ballouli's Blog
description: Rim El Ballouli's personal blog
author: Rim El Ballouli
social:
  links:
    - https://www.linkedin.com/in/rim-el-ballouli/
    - https://github.com/Rim-El-Ballouli/
    - https://www.researchgate.net/profile/Rim_El_Ballouli2/
    - https://scholar.google.com/citations?hl=en&user=ifD1gh0AAAAJ
lang: en_US
---
<h1>Posts</h1>
{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
    <li>
     <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
  </ul>
{% endfor %}