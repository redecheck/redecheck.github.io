---
layout: post
title: "Covered-Calendar Failure 5"
permalink: Covered-Calendar-failure-5
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 30 | 768px-979px | TP | Header navigation link clearly wraps onto a new line | 

![Screenshot of the fault](assets/images/Covered-Calendar/fault5/wrappingWidth873.png){: .center-image }

## About Distinct RLF 30 {#About-drlf}

The "Pricing" navigation link in the header bar wraps onto a new line as the viewport becomes narrow. Given the failure manifests right at the top of the webpage, it should be a high-priority fix for the developer to ensure the issue does not negatively influence visitors to the site.

The issue manifests on many viewport widths and is located at the top of the web page. Therefore, a manual testing procedure would likely detect it with relative ease. Despite this, the issue is still present on the live version of the site, [here](https://www.coveredcalendar.com/).

At mobile widths, the navigation links are collapsed to a drop-down menu:
![Mobile](assets/good-bad/rlf30/mobile.png){: .center-image}

Here is the failure manifesting:
![Bad](assets/good-bad/rlf30/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](assets/good-bad/rlf30/ok.png){: .center-image}
