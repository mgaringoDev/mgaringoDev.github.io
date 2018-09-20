---
layout: default
title: Software Development
category: projectSummarypage
---

# List of {{page.title}}  Projects

<div style="width: 100%;">
  <p align="center" >
    <font size="2.1em">              
    	&#9670;
      {% for pages in site.pages%}
        {% if pages.category == "projectSummarypage" %}
          <a href="{{pages.url}}" style="padding: 5px;">{{pages.title}}</a>          
          &#9670;          
        {% endif %}                
      {% endfor %}                
    </font>
  </p>
</div>

<hr>

## Software Development
{% for post in site.posts %}
{% if post.tags contains 'SoftwareDevelopment' %}
- [{{post.title}}]({{post.url}})
{% endif %}
{% endfor %}