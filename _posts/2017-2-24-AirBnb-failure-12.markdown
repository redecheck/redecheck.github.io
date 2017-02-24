---
layout: post
title: "AirBnb Failure 12"
permalink: AirBnb-failure-12
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 26 | 321px-335px | TP | 'Terms and Privacy' clearly wrapped onto new row | 

![Screenshot of the fault](assets/images/AirBnb/fault12/wrappingWidth328.png){: .center-image }

## About Distinct RLF 26 {#About-drlf}

‘Terms & Privacy’ icon wraps onto a new line. Not a major issue at all, but something the developer may want to remedy. Please note, the highlighting on the image produced by the tool indicates the wrapped element is actually overlapping with some of the other elements. This is not the case, and is simply due to the width of the boxes used to highlight the offending elements making them appear to be overlapping. 

It is only visible for a few viewport widths and is also located in the footer of a long web page, so manual testing would likely find it difficult to detect.

An update to the [live version](http://airbnb.com) of the page means this failure no longer manifests.

Here is the failure manifesting:
![Bad](assets/good-bad/rlf26/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](assets/good-bad/rlf26/ok.png){: .center-image}
