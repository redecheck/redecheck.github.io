---
layout: post
title: "HotelWifiTest Failure 1"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 20 | 415px-767px | TP | Main container clearly protruding from the viewport, obscuring lots of content | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/HotelWifiTest/fault1/viewportOverflowWidth591.png){: .center-image }

## About Distinct RLF 20

At narrow, mobile-device widths, the main content panels of the web page are displayed in two columns. However, beyond the viewport width of 414px, this shifts to a 4 column layout, despite the viewport not being anywhere near wide enough to accommodate the items. This causes almost half of the main content of the web page to protrude outside of the viewport, giving the web page quite an unprofessional aesthetic. Although a user could scroll horizontally to view the rest of the content, many web users nowadays do not expect to scroll horizontally, they may not realise they have the ability to do so and simply disregard the obscured information.

At mobile widths, a simple two column layout is used:
![380px]({{ site.baseurl }}/assets/good-bad/rlf20/380.png){: .center-image}

At slightly wider widths, the layout switches but there is not enough room:
![430px]({{ site.baseurl }}/assets/good-bad/rlf20/430.png){: .center-image}

At wider viewports, there is enough room and all is well
![1024px]({{ site.baseurl }}/assets/good-bad/rlf20/1024.png){: .center-image}
