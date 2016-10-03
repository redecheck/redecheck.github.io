---
layout: page
title: ICST 2017
permalink: /icst17/
---

**In our previous [ASE paper](http://redecheck.org/publications/)** we introduced the "Responsive Layout Graph", which models the layout of a responsive web page, and showed how it could be used to detect (potentially unintended) changes to a website.

**In our ICST 2017 submission**, we propose four algorithms that can be used with the RLG to detect common types of layout failure ("responsive layout failures"). These common failure types are described in the submission, and include element overlap, element and viewport overflow, small-range layouts and wrapping. We conducted an empirical study on 25 live and active subject web pages, including Airbnb, Pocket and Stumbleupon amongst others.

The links below give further details of each of the failure reports raised by our ReDeCheck tool, a screenshot showing the HTML elements identified, and its classification (TP, FP or NOI):


| Title | URL | HTML Elements | CSS Declarations | Results |
|---|---|{% for my_post in site.posts reversed %}{% if my_post.title %}
|{{ my_post.title }}  |{{ my_post.fullurl }}  | {{my_post.elements }} | {{ my_post.decs }} | [Click Here]({{ my_post.url }}){% endif %}{% endfor %}