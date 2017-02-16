---
layout: post
title: "3-Minute-Journal Fault 3"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 13 | 992px-1136px | TP | 'July' label outside the viewport | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault3/viewportOverflowWidth1064.png){: .center-image }

## About Distinct RLF 13

Graph protrudes outside viewport again, this time at narrow widths. Given the graph is already below the text, the only option to the developer is to implement a fluid width for the element to stop it protruding from the viewport. As it manifests at many viewport widths including several common mobile resolutions, it should be easy to detect manually.

Below is the webpage with the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf13/bad.png){: .center-image }

When the viewport gets wider, all is well:
![OK]({{ site.baseurl }}/assets/good-bad/rlf13/ok.png){: .center-image }
