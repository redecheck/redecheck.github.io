---
layout: post
title: "Pdf-Escape Failure 8"
permalink: Pdf-Escape-failure-8
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Protrusion| 11 | 801px-805px | TP | Navigation links have clearly protruded outside the navbar and become invisible and unclickable | 

![Screenshot of the fault](../assets/images/Pdf-Escape/fault8/overflow-Width803.png){: .center-image }

## About Distinct RLF 11 {#About-drlf}

At narrow widths, the navigation links in the web page's header are collapsed down to a drop down list which can be revealed by clicking on a button. At wider widths, the links expand into a row of elements. However, for a small number of widths after the layout changes to a row of elements, there is insufficient space in the header and the elements overflow the header. As the header has the `overflow: hidden` CSS property set, the overflowing links are invisible and unclickable at this small range of widths. This could have detrimental impacts as any users to the site at this viewport size could think that the home page is the only page available on the site.

Given that it occurs for such a small number of widths and these widths are "in between" typical tablet and desktop viewport sizes, it is likely the fault would go undetected by manual testing. Indeed, the failure is still present in the live version of the site, available [here](http://www.pdfescape.com/).

The links collapsed to a drop down:
![760px](../assets/good-bad/rlf11/760.png){: .center-image}

At a small range of widths, the elements overflow and are unclickable:
![802px](../assets/good-bad/rlf11/802.png){: .center-image}

At wider widths, they are correctly rendered in a row in the header:
![1024px](../assets/good-bad/rlf11/1024.png){: .center-image}
