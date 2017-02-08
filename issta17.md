---
layout: page
title: ISSTA 2017
permalink: /issta17/
---

**In our previous [ASE paper](http://redecheck.org/publications/)** we introduced the "Responsive Layout Graph", which models the layout of a responsive web page, and showed how it could be used to detect (potentially unintended) changes to a website.

**In our ISSTA 2017 submission**, we propose four algorithms that can be used with the RLG to detect common types of layout failure ("responsive layout failures"). These common failure types are described in the submission, and include element overlap, element and viewport overflow, small-range layouts and wrapping. We conducted an empirical study on 25 live and active subject web pages, including _Airbnb_, _Pocket_, and _Stumbleupon_ amongst others.

## Research Question One
The links below give further details of each of the failure reports raised by our ReDeCheck tool, a screenshot showing the HTML elements identified, and its classification (TP, FP or NOI).

| Title | URL | HTML Elements | CSS Declarations | Results |
|---|---|{% for my_post in site.posts reversed %}{% if my_post.title %}
|{{ my_post.title }}  |[{{ my_post.fullurl }}](http://{{ my_post.fullurl }})  | {{my_post.elements }} | {{ my_post.decs }} | [Click Here]({{ my_post.url }}){% endif %}{% endfor %}

## Research Question Two
A spreadsheet showing which responsive layout failures can be observed at various viewport widths can be downloaded as an [Excel]({{ site.baseurl }}/assets/rq2.xlsx) or as a [CSV]({{ site.baseurl }}/assets/rq2.csv).

## Research Question Three
An archive containing all the individual timing results for our prototype tool is available for download [here]({{ site.baseurl }}/assets/times.zip). PLEASE NOTE: the times recorded are made up of three stages, so the times plotted in the paper correspond to the SUM of these three values.
