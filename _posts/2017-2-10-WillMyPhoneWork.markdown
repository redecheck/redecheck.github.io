---
layout: post
title: "WillMyPhoneWork"
elements: 781
decs: 2022
fullurl: willmyphonework.net
---

| RLF No. | Type | Description | Screenshot (Bad) | Screenshot (OK) |
| 33 | Element Collision | Navigation links all get pushed onto a second line, causing the navigation bar to overlap with the main content. All the navigation links remain clickable, but as some information is obscured, we classify this a true positive. It appears that the media query which changed the navigation from a drop-down to a navbar needs modifying to 'toggle' at a slightly wider width to make sure there's enough room for the desired layout. As the failure only manifests for 2 viewport widths, neither of which are particularly common, it would likely be difficult for a manual tester to detect it. | [Bad]({{ site.baseurl }}/assets/good-bad/rlf33/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf33/ok.png) |


The failure still exists on the live site, as can be observed [here](http://WillMyPhoneWork.net).


| Failure No. | Category | Screenshot | Classification | Reason | Distinct RLF |
| 1| Element Collision | [Click]({{ site.baseurl }}/assets/images/WillMyPhoneWork/fault1/overlapWidth990.png) | TP | No visible content overlap, just DOM coordinates | 33 |
| 2| Element Protrusion | [Click]({{ site.baseurl }}/assets/images/WillMyPhoneWork/fault2/overflow-Width1095.png) | NOI | Element is not visibly protruding from its parent | |
| 3| Small-Range | [Click]({{ site.baseurl }}/assets/images/WillMyPhoneWork/fault3/smallrangeWidth990.png) | TP | Elements are only overlapping for a couple of widths, so a TP | 33|
| 4| Small-Range | [Click]({{ site.baseurl }}/assets/images/WillMyPhoneWork/fault4/smallrangeWidth990.png) | TP | Alignment only true for a couple of widths, so a TP | 33|
