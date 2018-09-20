---
layout: default
title: Projects
category: SidePanel
---
# List of Projects


{% for post in site.posts %}
{% if post.tags contains 'Buiness' %}

<li><a href="{{post.url}}">  {{post.title}}  </a></li>
{% endif %}
{% endfor %}

<!-- THIS IS WORKING

{% for post in site.posts %}

<li><a href="{{post.url}}">  {{post.title}}  </a></li>

{% endfor %}
-->
		

