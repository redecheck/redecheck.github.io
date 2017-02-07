---
layout: page
title: ISSTA 2017
permalink: /issta17/
---

**In our ISSTA 2017 submission**, we propose four algorithms that can be used with the RLG to detect common types of layout failure ("responsive layout failures") without the use of explicit oracles. These common failure types are described in the submission, and include element collision, element and viewport protrusion, small-range layouts and wrapping. We conducted an empirical study on 26 live and active subject web pages, including _Airbnb_, _Pocket_, and _Stumbleupon_ amongst others.

The links below give further details of each of the failure reports raised by our ReDeCheck tool, a screenshot showing the HTML elements identified, its classification (TP, FP or NOI) and the reasoning behind the classification.

| Title | URL | HTML Elements | CSS Declarations | Results |
|---|---|{% for my_post in site.posts reversed %}{% if my_post.title %}
|{{ my_post.title }}  |[{{ my_post.fullurl }}](http://{{ my_post.fullurl }})  | {{my_post.elements }} | {{ my_post.decs }} | [Click Here]({{ my_post.url }}){% endif %}{% endfor %}
