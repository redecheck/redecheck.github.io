---
layout: post
title: "Covered-Calendar Failure 4"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 29 | 320px-385px | TP | 'Privacy Policy' cleared wraps onto a new line | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/Covered-Calendar/fault4/wrappingWidth352.png){: .center-image }

## About Distinct RLF 29

The "Privacy Policy" links wraps onto a new line as the viewport becomes narrow. As the vertical bar has also wrapped, it indicates the wrapping is not intended layout behaviour, as the "CoveredCalendar.com" link doesn't have a bar on its left hand side. The developer could implement either fluid widths on the links or simply reduce the padding between the links to resolve the issue.

The issue manifests on many common mobile device viewport widths, but the failure is located at the bottom of the web page. Therefore, a fairly thorough manual testing procedure would likely be required to detect it.

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf29/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf29/ok.png){: .center-image}
