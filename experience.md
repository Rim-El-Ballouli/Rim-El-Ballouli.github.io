---
layout: default
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