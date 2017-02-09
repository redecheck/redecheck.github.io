---
layout: page
title: ISSTA 2017
permalink: /issta17/
---

## Distinct Responsive Layout Failures

| RLF No. | Web Page | Type | Description | Screenshot (Bad) | Screenshot (OK) |
| 1 | 3-Minute-Journal | Viewport Protrusion | Graph protrudes outside viewport | [Click]({{ site.baseurl }}/assets/good-bad/rlf1/bad.png) | [Click]({{ site.baseurl }}/assets/good-bad/rlf1/good.png) |
| 2 | 3-Minute-Journal | Viewport Protrusion | Graph protrudes outside viewport again | [Click]({{ site.baseurl }}/assets/good-bad/rlf2/bad.png) | [Click]({{ site.baseurl }}/assets/good-bad/rlf2/good.png) |


## Research Question One
The links below give further details of each of the failure reports raised by our ReDeCheck tool, a screenshot showing the HTML elements identified, and its classification (TP, FP or NOI).

| Title | URL | HTML Elements | CSS Declarations | Results |
|---|---|{% for my_post in site.posts reversed %}{% if my_post.title %}
|{{ my_post.title }}  |[{{ my_post.fullurl }}](http://{{ my_post.fullurl }})  | {{my_post.elements }} | {{ my_post.decs }} | [Click Here]({{ my_post.url }}){% endif %}{% endfor %}

## Research Question Two
A spreadsheet showing which responsive layout failures can be observed at various viewport widths can be downloaded as an [Excel]({{ site.baseurl }}/assets/rq2.xlsx) or as a [CSV]({{ site.baseurl }}/assets/rq2.csv).

## Research Question Three
A .CSV file containing all of the timing results for our prototype tool is available for download [here]({{ site.baseurl }}/assets/times.csv). PLEASE NOTE: the times recorded are made up of three stages, so the times plotted in the paper correspond to the SUM of these three values. An R snippet to reproduce the graph seen in the paper is available [here]().
