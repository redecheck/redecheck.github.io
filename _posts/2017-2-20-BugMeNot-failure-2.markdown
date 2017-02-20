---
layout: post
title: "BugMeNot Failure 2"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 15 | 320px-340px | TP | Part of input box obscured by viewport protrusion, so a TP | 

![Screenshot of the fault](../../../assets/images/BugMeNot/fault2/viewportOverflowWidth330.png){: .center-image }

## About Distinct RLF 15

At narrow viewport widths, the static width of the form field means it protrudes outside of the viewport on the left hand side. While not detrimentally affecting the functionality of the page, it does have a negative impact on the aesthetics of the page, which could influence any visitors to the site.

The failure is only visible for a fairly small number of viewport widths, but the very common viewport width of 320px is one of them. As the failure is also clearly visible right at the top of the page, a manual testing procedure should be easily able to detect it. However, it is still currently present on the live version of the site, available [here](http://bugmenot.com/).

Here is the web page when the failure is not manifesting:
![OK](../../../assets/good-bad/rlf15/ok.png){: .center-image}

At 320px, the form field is overflowing the viewport quite significantly:
![Bad](../../../assets/good-bad/rlf15/bad.png){: .center-image}
