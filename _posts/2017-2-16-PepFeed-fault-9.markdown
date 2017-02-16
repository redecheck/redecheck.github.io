---
layout: post
title: "PepFeed Fault 9"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 5 | 769px-933px | TP | Panels 1 and 3 clearly overlapping | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/PepFeed/fault9/overlapWidth851.png){: .center-image }

## About Distinct RLF 5

When the viewport is wide such as on a desktop, four content panels are rendered side by side. However, in between these widths one of the panels shifts onto a new row and two of the panels overlap, obscuring some of the content. As the failure occurs at the top of the page, it makes the page look very unprofessional and has the potential to discourage visitors from using the service provided.

Given that the failure manifests on a reasonable number of viewport widths and is located near the top of the page, it should be easily detected by a manual tester. However, the faulty viewport widths are "in between" typical smartphone and tablet sizes, which might explain why the fault is still manifesting in the live site, available [here](http://pepfeed.com).

At 1000px, the layout is in a row and all is well:
![1000px]({{ site.baseurl }}/assets/good-bad/rlf5/1000.png){: .center-image}

However, an narrow viewport widths such as 928px, an overlap occurs
![928px]({{ site.baseurl }}/assets/good-bad/rlf5/928.png){: .center-image}
