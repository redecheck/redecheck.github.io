---
layout: post
title: "UserSearch Failure 2"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 33 | 625px-794px | TP | Final navigation link clearly wrapped onto a new line | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/UserSearch/fault2/wrappingWidth709.png){: .center-image }

## About Distinct RLF 33

The navigation links wrap incongruously onto different lines as the viewport becomes narrow. While clearly not a major issue, it is something the developer may want to address nonetheless as makes the page appear significantly less professional, as many people now expect a mobile-ready "drop-down" menu rather than a desktop menu which has wrapped.

The issue manifests on many device viewport widths and is part of the page's main content, so a manual testing procedure should be able to detect it easily. Despite this, the issue is still present on the live version of the site, [here](https://usersearch.org/).

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf33/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf33/ok.png){: .center-image}
