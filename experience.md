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
<h1> Research Experience </h1>
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'research' %}
    <li>
      <h3>{{ exp.job_title }} </h3> at {{ exp.company }} <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      <div class="exp-list"><ul>
      {{ exp.content | markdownify }}
      </ul></div>
    </li>
    {% endif %}
  {% endfor %}
</ul> 


<h1> Industry Experience</h1>
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'indusrty' %}
    <li>
      <h3> {{ exp.job_title }} </h3> at {{ exp.company }} <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      <div class="exp-list"><ul>
      {{ exp.content | markdownify }}
      </ul></div>
    </li>
    {% endif %}
  {% endfor %}
</ul> 


<h1> Teaching Experience</h1>
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'teaching' %}
    <li>
      <h3> {{ exp.job_title }} </h3> at {{ exp.company }} <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      <div class="exp-list"><ul>
      {{ exp.content | markdownify }}
      </ul></div>
    </li>
    {% endif %}
  {% endfor %}
</ul> 