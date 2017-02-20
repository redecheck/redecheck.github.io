---
layout: post
title: "Pdf-Escape Failure 4"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 21 | 768px-850px | TP | Part of image obscured by protrusion outside viewport | 

![Screenshot of the fault](../../../assets/images/Pdf-Escape/fault4/viewportOverflowWidth809.png){: .center-image }

## About Distinct RLF 21

At wide viewport widths, the row of company logos are rendered easily side-by-side However, as the viewport starts to narrow, the "PCWorld" logo starts to protrude outside of the viewport. While this does not hamper functionality, the visual appearance is sub-optimal, as there is clearly supposed to be white space on the right hand side of the row of logos, but instead part of one of the logos is obscured.

The failure only manifests for a fairly small range of viewport widths, which are not commonly advocated for testing, so a manual testing procedure may struggle to easily detect it. It is still currently present on the live version of the site, available [here](http://www.pdfescape.com/).

Here is the web page when the failure is not manifesting:
![OK](../../../assets/good-bad/rlf21/ok.png){: .center-image}

At narrower viewport widths, the image protrudes out of the viewport:
![Bad](../../../assets/good-bad/rlf21/bad.png){: .center-image}
