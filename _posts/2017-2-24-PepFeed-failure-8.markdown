---
layout: post
title: "PepFeed Failure 8"
permalink: PepFeed-failure-8
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 4 | 547px-700px | TP | Panels 1 and 3 clearly overlapping | 

![Screenshot of the fault](../assets/images/PepFeed/fault8/overlapWidth623.png){: .center-image }

## About Distinct RLF 4 {#About-drlf}

When the viewport is wide enough, three content panels are rendered side by side. However, in between these widths two of the panels overlap, obscuring some of the content. As the failure occurs at the top of the page, it makes the page look very unprofessional and has the potential to discourage visitors from using the service provided.

Given that the failure manifests on a reasonable number of viewport widths and is located near the top of the page, it should be easily detected by a manual tester. However, the faulty viewport widths are "in between" typical smartphone and tablet sizes, which might explain why the fault is still manifesting in the live site, available [here](http://pepfeed.com).

At 750px, the layout is in a row and all is well:
![750px](../assets/good-bad/rlf4/750.png){: .center-image}

However, an narrow viewport widths, an overlap occurs
![650px](../assets/good-bad/rlf4/650.png){: .center-image}
