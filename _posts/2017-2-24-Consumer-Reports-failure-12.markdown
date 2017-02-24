---
layout: post
title: "Consumer-Reports Failure 12"
permalink: Consumer-Reports-failure-12
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 16 | 320px-375px | TP | Element clearly protruding outside of the viewport | 

![Screenshot of the fault](assets/images/Consumer-Reports/fault12/viewportOverflowWidth347.png){: .center-image }

## About Distinct RLF 16 {#About-drlf}

At wider viewport widths, the "Featured Products" tiles fit comfortably within the viewport window. However, at narrow viewport widths, they begin to protrude outside of it. While initially this means just obscuring the white space on the right hand side of the tiles, as the viewport narrows further text begins to become obscured, making the web page look considerably less professional.

The failure is only visible for a fairly small number of viewport widths, but the very common viewport width of 320px is one of them. As the failure is also clearly visible (multiple tiles all protruding in the middle of the page), a manual testing procedure should be easily able to detect it. However, it is still currently present on the live version of the site, available [here](http://bugmenot.com/).

Here is the web page when the failure is not manifesting:
![OK](assets/good-bad/rlf16/ok.png){: .center-image}

The tiles begin to protrude, but not significantly:
![Bad](assets/good-bad/rlf16/bad.png){: .center-image}

At 320px, the tiles overflowing the viewport quite significantly:
![Very Bad](assets/good-bad/rlf16/verybad.png){: .center-image}
