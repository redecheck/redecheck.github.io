---
layout: post
title: "3-Minute-Journal Failure 7"
permalink: 3-Minute-Journal-failure-7
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 13 | 992px-1055px | TP | 'Jun' label outside the viewport | 

![Screenshot of the fault](assets/images/3-Minute-Journal/fault7/viewportOverflowWidth1023.png){: .center-image }

## About Distinct RLF 13 {#About-drlf}

Graph protrudes outside viewport again, this time at narrow widths. Given the graph is already below the text, the only option to the developer is to implement a fluid width for the element to stop it protruding from the viewport. As it manifests at many viewport widths including several common mobile resolutions, it should be easy to detect manually.

Below is the webpage with the failure manifesting:
![Bad](assets/good-bad/rlf13/bad.png){: .center-image }

When the viewport gets wider, all is well:
![OK](assets/good-bad/rlf13/ok.png){: .center-image }
