---
layout: post
title: "Consumer-Reports Failure 14"
permalink: Consumer-Reports-failure-14
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Protrusion| 10 | 392px-767px | TP | Text has clearly protruding outside its container | 

![Screenshot of the fault](../assets/images/Consumer-Reports/fault14/overflow-Width579.png){: .center-image }

## About Distinct RLF 10 {#About-drlf}

At wider viewport widths, the text "All Products A-Z" is correctly rendered inside its containing element. However, at narrower widths, mistakes in the CSS cause it to overflow its container, producing poor aesthetics which could have a detrimental impact on user confidence in the site.

As it manifests at a large number of viewport widths, including many mobile device widths, it should be relatively easy to detect with a manual testing approach. However, the failure is still manifesting in the live site, available [here](http://www.consumerreports.org/cro/index.htm).

At wider widths, the text fits within its container correctly:
![980px](../assets/good-bad/rlf10/980.png){: .center-image}

However, at narrower ones, the text overflows:
![760px](../assets/good-bad/rlf10/760.png){: .center-image}
