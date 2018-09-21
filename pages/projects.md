---
layout: default
title: Projects
category: SidePanel
---
# List of All Projects

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

## Research

{% for post in site.posts %}
{% if post.tags contains 'Research' %}
<ul style="margin:0.5em;">
  <li>
    <a href='{{post.url}}'>
      {{post.title}}
    </a>
  </li>
</ul>
{% endif %}
{% endfor %}


<br>

## Business
{% for post in site.posts %}
{% if post.tags contains 'Business' %}
<ul style="margin:0.5em;">
  <li>
    <a href='{{post.url}}'>
      {{post.title}}
    </a>
  </li>
</ul>
{% endif %}
{% endfor %}

<br>

## Software Development
{% for post in site.posts %}
{% if post.tags contains 'SoftwareDevelopment' %}
<ul style="margin:0.5em;">
  <li>
    <a href='{{post.url}}'>
      {{post.title}}
    </a>
  </li>
</ul>
{% endif %}
{% endfor %}



<!-- THIS IS WORKING

{% for post in site.posts %}

<li><a href="{{post.url}}">  {{post.title}}  </a></li>

{% endfor %}
-->
		

