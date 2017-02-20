---
layout: post
title: "Consumer-Reports Failure 6"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 18 | 768px-1039px | TP | Element clearly protruding outside of the viewport | 

![Screenshot of the fault](../../../assets/images/Consumer-Reports/fault6/viewportOverflowWidth903.png){: .center-image }

## About Distinct RLF 18

At wide viewport widths, the "Price Watch" and "Featured" tiles easily fit side-by-side in the main content banner of the page. However, as the viewport starts to narrow, the static widths of the two tiles means the "Featured" tile starts to protrude outside of the viewport, obscured a large portion of its content. Although a user could scroll horizontally in a carousel-like fashion to view the rest of the content, this seems to be a poor design choice given there are only two elements. Also, as many web users nowadays do not expect to scroll horizontally, they may not realise they have the ability to do so and simply disregard the obscured information.

The failure is visible for many viewport widths and is located at the top of the page, so a manual testing procedure should easily detect it. However, it is still currently present on the live version of the site, available [here](http://bugmenot.com/).

Here is the web page when the failure is not manifesting:
![OK](../../../assets/good-bad/rlf18/ok.png){: .center-image}

At narrower viewport widths, the "Featured" tile significantly protrudes out of the viewport:
![Bad](../../../assets/good-bad/rlf18/bad.png){: .center-image}
