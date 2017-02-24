---
layout: post
title: "Ninite Failure 2"
permalink: Ninite-failure-2
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 31 | 347px-395px | TP | 'terms' nav link clearly wrapped onto new line | 

![Screenshot of the fault](assets/images/Ninite/fault2/wrappingWidth371.png){: .center-image }

## About Distinct RLF 31 {#About-drlf}

The "terms" links wraps onto a new line as the viewport becomes narrow. While clearly not a major issue, it is something the developer may want to address nonetheless. The developer could implement either fluid widths on the links or simply reduce the padding between the links to resolve the issue.

The issue manifests on some common mobile device viewport widths, but the failure is located at the bottom of the web page. Therefore, a fairly thorough manual testing procedure would likely be required to detect it. Indeed, the issue is still present on the live version of the site, [here](https://ninite.com/).

Here is the failure manifesting:
![Bad](assets/good-bad/rlf31/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](assets/good-bad/rlf31/ok.png){: .center-image}
