---
layout: post
title: "PepFeed Failure 28"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 32 | 320px-386px | TP | 'The Verge' has clearly wrapped onto a new line | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/PepFeed/fault28/wrappingWidth353.png){: .center-image }

## About Distinct RLF 32

The "Verge" link wraps onto a new line as the viewport becomes narrow. While clearly not a major issue, it is something the developer may want to address nonetheless. The developer could implement a large width on the container to stop the failure from occurring.

The issue manifests on some common mobile device viewport widths, so a fairly thorough manual testing procedure should be able to detect it. Indeed, the issue is still present on the live version of the site, [here](https://pepfeed.com/).

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf32/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf32/ok.png){: .center-image}
