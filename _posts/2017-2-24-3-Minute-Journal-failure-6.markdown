---
layout: post
title: "3-Minute-Journal Failure 6"
permalink: 3-Minute-Journal-failure-6
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 12 | 320px-542px | TP | 'Jun' label outside the viewport | 

![Screenshot of the fault](../assets/images/3-Minute-Journal/fault6/viewportOverflowWidth431.png){: .center-image }

## About Distinct RLF 12 {#About-drlf}

Graph protrudes outside viewport. As the graph has a fixed width and the developer wants to render it side-by-side with the main text, the graph should either have a fluid width or a media query should change the alignment of the elements before the failure occurs (e.g. render the graph below the text). As the failure manifests for around 150px and is viewable at the common viewport width of 1024px, a reasonable manual testing approach should be able to detect it.

Below is the webpage with the failure manifesting:
![Bad screenshot](../assets/good-bad/rlf12/bad.png){: .center-image }

When the viewport gets wider, all is well:
![OK](../assets/good-bad/rlf12/ok.png){: .center-image }
