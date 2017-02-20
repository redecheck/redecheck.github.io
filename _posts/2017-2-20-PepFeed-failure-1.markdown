---
layout: post
title: "PepFeed Failure 1"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 22 | 415px-768px | TP | Amazon logo obscured by viewport at narrower width than screenshot. | 

![Screenshot of the fault](../../../assets/images/PepFeed/fault1/viewportOverflowWidth591.png){: .center-image }

## About Distinct RLF 22

At wide viewport widths, the row of company logos are rendered easily side-by-side However, as the viewport starts to narrow, the "Amazon" logo starts to protrude outside of the viewport. While this does not hamper functionality, the visual appearance is sub-optimal, as there is clearly supposed to be white space on the right hand side of the row of logos, but instead part of one of the logos is obscured.

At the DOM coordinate level, the failure manifests for many viewport widths, but visually the logo is only obscured for a few viewport widths, so a manual testing procedure may struggle to easily detect it. It is still currently present on the live version of the site, available [here](http://www.pepfeed.com/).

Here is the web page when the failure is not manifesting:
![OK](../../../assets/good-bad/rlf22/ok.png){: .center-image}

At narrower viewport widths, the image protrudes out of the viewport:
![Bad](../../../assets/good-bad/rlf22/bad.png){: .center-image}
