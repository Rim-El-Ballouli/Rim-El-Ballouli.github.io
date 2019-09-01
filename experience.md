---
layout: default
---
<span class="exp-type"> Research Experience </span>
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'research' %}
    <li>
      <span class="job-title"> {{ exp.job_title }} </span> at {{ exp.company }} <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      <div class="exp-list"><ul>
      {{ exp.content | markdownify }}
      </ul></div>
    </li>
    {% endif %}
  {% endfor %}
</ul> 


<span class="exp-type"> Industry Experience</span>
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'indusrty' %}
    <li>
      <span class="job-title"> {{ exp.job_title }} </span> at {{ exp.company }} <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      <div class="exp-list"><ul>
      {{ exp.content | markdownify }}
      </ul></div>
    </li>
    {% endif %}
  {% endfor %}
</ul> 


<span class="exp-type"> Teaching Experience</span>
<ul>
  {% for exp in site.experience %}
  {% if exp.type == 'teaching' %}
    <li>
      <span class="job-title"> {{ exp.job_title }} </span> at {{ exp.company }} <br/>
      {{ exp.start_date }} - {{ exp.end_date }}<br/>
      {{ exp.location }} 
      <div class="exp-list"><ul>
      {{ exp.content | markdownify }}
      </ul></div>
    </li>
    {% endif %}
  {% endfor %}
</ul> 