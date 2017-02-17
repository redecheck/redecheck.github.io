---
layout: post
title: "AirBnb Failure 13"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 27 | 326px-356px | TP | Instagram logo clearly wrapped onto new row | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/AirBnb/fault13/wrappingWidth341.png){: .center-image }

## About Distinct RLF 27

Instagram icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row. Manifests at the bottom of a long web page for fairly few viewport widths, so would likely go unnoticed by a manual testing procedure.

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf27/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf27/ok.png){: .center-image}
