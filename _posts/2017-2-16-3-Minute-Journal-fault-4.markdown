---
layout: post
title: "3-Minute-Journal Fault 4"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 12 | 320px-413px | TP | 'Mar' label outside the viewport | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault4/viewportOverflowWidth366.png){: .center-image }

## About Distinct RLF 12

Graph protrudes outside viewport. As the graph has a fixed width and the developer wants to render it side-by-side with the main text, the graph should either have a fluid width or a media query should change the alignment of the elements before the failure occurs (e.g. render the graph below the text). As the failure manifests for around 150px and is viewable at the common viewport width of 1024px, a reasonable manual testing approach should be able to detect it.

Below is the webpage with the failure manifesting:
![Bad screenshot]({{ site.baseurl }}/assets/good-bad/rlf12/bad.png){: .center-image }

When the viewport gets wider, all is well:
![OK]({{ site.baseurl }}/assets/good-bad/rlf12/ok.png){: .center-image }
