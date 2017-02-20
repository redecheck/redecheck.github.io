---
layout: post
title: "StumbleUpon Failure 1"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 7 | 320px-439px | TP | Element collision clearly causing undesirable layout | 

![Screenshot of the fault](../../../assets/images/StumbleUpon/fault1/overlapWidth379.png){: .center-image }

## About Distinct RLF 7

When the viewport is wide enough, the login link is rendered in the top right corner and the company logo is rendered in the centre of the page, just beneath it. However, as the viewport narrows, the login link is forced to wrap slightly and pushes the logo over to the left hand side of the page. Even there being no strict overlap of content, the layout shift has clearly caused an incongrous layout, rather than just a DOM level overlap.

Given that the failure manifests on a reasonable number of viewport widths including many common mobile device viewport widths and is located near the top of the page, it should be easily detected by a manual tester. However, the fault is still manifesting in the live site, available [here](http://www.stumbleupon.com/).

At 476px, all is well with the layout:
![476px](../../../assets/good-bad/rlf7/476.png){: .center-image}

However, an narrow viewport widths such as 395px, an overlap occurs, causing the undesirable layout:
![395px](../../../assets/good-bad/rlf7/395.png){: .center-image}
