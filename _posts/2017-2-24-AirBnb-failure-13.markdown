---
layout: post
title: "AirBnb Failure 13"
permalink: AirBnb-failure-13
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 27 | 326px-356px | TP | Instagram logo clearly wrapped onto new row | 

![Screenshot of the fault](assets/images/AirBnb/fault13/wrappingWidth341.png){: .center-image }

## About Distinct RLF 27 {#About-drlf}

Instagram icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row. Manifests at the bottom of a long web page for fairly few viewport widths, so would likely go unnoticed by a manual testing procedure.

Here is the failure manifesting:
![Bad](assets/good-bad/rlf27/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](assets/good-bad/rlf27/ok.png){: .center-image}
