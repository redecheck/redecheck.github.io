---
layout: page
title: ISSTA 2017
permalink: /issta17/
---

## Distinct Responsive Layout Failures


| RLF No. | Web Page | Type | Description | Screenshots |
| 1 | 3-Minute-Journal | Viewport Protrusion | Graph protrudes outside viewport | [Bad]({{ site.baseurl }}/assets/good-bad/rlf1/bad.png)  [OK]({{ site.baseurl }}/assets/good-bad/rlf1/ok.png) |
| 2 | 3-Minute-Journal | Viewport Protrusion | Graph protrudes outside viewport again | [Bad]({{ site.baseurl }}/assets/good-bad/rlf2/bad.png)  [OK]({{ site.baseurl }}/assets/good-bad/rlf2/ok.png) |
| 3 | AccountKiller | Small-Range | Some tiles shift location for 476px-480px. While not strictly 'bad' in terms of aesthetics, notifying a developer of this layout shift would likely still be useful | [475px]({{ site.baseurl }}/assets/good-bad/rlf3/475.png)  [478px]({{ site.baseurl }}/assets/good-bad/rlf3/478.png)  [481px]({{ site.baseurl }}/assets/good-bad/rlf3/481.png) |
| 4 | AccountKiller | Wrapping | 'The Atlantic' wraps onto a new line. No impact on functionality, but aesthetically, two rows of three icons might look much more professional | [Bad]({{ site.baseurl }}/assets/good-bad/rlf4/bad.png)  [OK]({{ site.baseurl }}/assets/good-bad/rlf4/ok.png) |
| 5 | AccountKiller | Wrapping | 'Tweet' icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row | [Bad]({{ site.baseurl }}/assets/good-bad/rlf5/bad.png)  [OK]({{ site.baseurl }}/assets/good-bad/rlf5/ok.png) |
| 6 | AirBnb | Wrapping | 'Terms & Privacy' icon wraps onto a new line. Not a major issue at all, but something the developer may want to remedy | [Bad]({{ site.baseurl }}/assets/good-bad/rlf6/bad.png)  [OK]({{ site.baseurl }}/assets/good-bad/rlf6/ok.png) |
| 7 | AirBnb | Wrapping | Instagram icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row | [Bad]({{ site.baseurl }}/assets/good-bad/rlf7/bad.png)  [OK]({{ site.baseurl }}/assets/good-bad/rlf7/ok.png) |

## Research Question One
The links below give further details of each of the failure reports raised by our ReDeCheck tool, a screenshot showing the HTML elements identified, and its classification (TP, FP or NOI).

| Title | URL | HTML Elements | CSS Declarations | Results |
|---|---|{% for my_post in site.posts reversed %}{% if my_post.title %}
|{{ my_post.title }}  |[{{ my_post.fullurl }}](http://{{ my_post.fullurl }})  | {{my_post.elements }} | {{ my_post.decs }} | [Click Here]({{ my_post.url }}){% endif %}{% endfor %}

## Research Question Two
A spreadsheet showing which responsive layout failures can be observed at various viewport widths can be downloaded as an [Excel]({{ site.baseurl }}/assets/rq2.xlsx) or as a [CSV]({{ site.baseurl }}/assets/rq2.csv).

## Research Question Three
A .CSV file containing all of the timing results for our prototype tool is available for download [here]({{ site.baseurl }}/assets/times.csv). PLEASE NOTE: the times recorded are made up of three stages, so the times plotted in the paper correspond to the SUM of these three values. An R snippet to reproduce the graph seen in the paper is available [here]().
