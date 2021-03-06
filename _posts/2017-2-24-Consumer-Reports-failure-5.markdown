---
layout: post
title: "Consumer-Reports Failure 5"
permalink: Consumer-Reports-failure-5
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Viewport Protrusion| 17 | 1025px-1110px | TP | Element clearly protruding outside of the viewport | 

![Screenshot of the fault](../assets/images/Consumer-Reports/fault5/viewportOverflowWidth1067.png){: .center-image }

## About Distinct RLF 17 {#About-drlf}

At wider viewport widths, the navigation links in the footer fit comfortably within the viewport window. However, at narrower viewport widths, one of the links (Privacy Policy) is fully obscured as the list protrudes out of the left side of the viewport. This means any user of the site at one of the faulty viewport widths would be unable to click on the link to read about the site's privacy policy, something many people are interested in nowadays.

The failure is only visible for a fairly small number of viewport widths and not at any commonly tested ones. As the failure is also located at the bottom of the page, a manual testing procedure may not detect it. However, it is still currently present on the live version of the site, available [here](http://bugmenot.com/).

Here is the web page when the failure is not manifesting:
![OK](../assets/good-bad/rlf17/ok.png){: .center-image}

The tiles begin to protrude, but not significantly:
![Bad](../assets/good-bad/rlf17/bad.png){: .center-image}
