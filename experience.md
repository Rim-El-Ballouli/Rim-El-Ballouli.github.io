---
layout: default
title: Experience
description: Rim El Ballouli's research, higher education, and industry experience
author: Rim El Ballouli
social:
  links:
    - https://www.linkedin.com/in/rim-el-ballouli/
    - https://github.com/Rim-El-Ballouli/
    - https://www.researchgate.net/profile/Rim_El_Ballouli2/
    - https://scholar.google.com/citations?hl=en&user=ifD1gh0AAAAJ
lang: en_US
---
# Research Experience 
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'research' %}
    <li>
      <strong> {{ exp.job_title }} </strong> at <em> {{ exp.company }} </em> <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      {{ exp.content | markdownify }}
    </li>
    {% endif %}
  {% endfor %}
</ul> 


# Industry Experience
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'indusrty' %}
    <li>
      <strong> {{ exp.job_title }} </strong> at <em> {{ exp.company }} </em><br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      {{ exp.content | markdownify }}
    </li>
    {% endif %}
  {% endfor %}
</ul> 


# Teaching Experience
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'teaching' %}
    <li>
      <strong> {{ exp.job_title }} </strong> at <em> {{ exp.company }} </em> <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      {{ exp.content | markdownify }}
    </li>
    {% endif %}
  {% endfor %}
</ul> 