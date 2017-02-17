---
layout: post
title: "Duolingo Failure 3"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 19 | 981px-1099px | TP | null | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/Duolingo/fault3/viewportOverflowWidth1040.png){: .center-image }

## About Distinct RLF 19

At wide viewport widths, the carousel of different languages easily fits in the main content banner of the page. However, as the viewport starts to narrow, the static widths of the carousel means the > arrow starts to protrude outside of the viewport, eventually becoming almost unclickable. This means users of the site may miss out on discovering the huge range of language courses offered by the site, so it is an issue which should be addressed.

The carousel protrudes outside of the viewport for many viewport widths, but the arrow is only obscured for a small number, so a manual testing procedure may struggle to easily detect it. However, it is still currently present on the live version of the site, available [here](https://www.duolingo.com/).

Here is the web page when the failure is not manifesting:
![OK]({{ site.baseurl }}/assets/good-bad/rlf19/ok.png){: .center-image}

At narrower viewport widths, the arrow protrudes out of the viewport and becomes almost unclickable:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf19/bad.png){: .center-image}
