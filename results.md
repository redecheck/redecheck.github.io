---
layout: page
title: ICST 2017
permalink: /icst17/
---

Below are links to the failure reports of the 25 subject web pages in our most recent study.
  	

| Title | URL | HTML Elements | CSS Declarations | Results |
|---|---|{% for my_post in site.posts reversed %}{% if my_post.title %}
|{{ my_post.title }}  |{{ my_post.fullurl }}  | {{my_post.elements }} | {{ my_post.decs }} | [Click Here]({{ my_post.url }}){% endif %}{% endfor %}