---
layout: post
title: "Covered-Calendar Failure 4"
permalink: Covered-Calendar-failure-4
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 29 | 320px-385px | TP | 'Privacy Policy' cleared wraps onto a new line | 

![Screenshot of the fault](../assets/images/Covered-Calendar/fault4/wrappingWidth352.png){: .center-image }

## About Distinct RLF 29 {#About-drlf}

The "Privacy Policy" links wraps onto a new line as the viewport becomes narrow. As the vertical bar has also wrapped, it indicates the wrapping is not intended layout behaviour, as the "CoveredCalendar.com" link doesn't have a bar on its left hand side. The developer could implement either fluid widths on the links or simply reduce the padding between the links to resolve the issue.

The issue manifests on many common mobile device viewport widths, but the failure is located at the bottom of the web page. Therefore, a fairly thorough manual testing procedure would likely be required to detect it.

Here is the failure manifesting:
![Bad](../assets/good-bad/rlf29/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](../assets/good-bad/rlf29/ok.png){: .center-image}
