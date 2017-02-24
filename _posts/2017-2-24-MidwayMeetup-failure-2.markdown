---
layout: post
title: "MidwayMeetup Failure 2"
permalink: MidwayMeetup-failure-2
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 2 | 768px-1132px | TP | Form is clearly overlapping with the main panel, and button is unclickable | 

![Screenshot of the fault](assets/images/MidwayMeetup/fault2/overlapWidth950.png){: .center-image }

## About Distinct RLF 2 {#About-drlf}

When the viewport is wide enough, two small forms are displayed side-by-side. However, as the viewport narrows, the responsive layout does not adjust accordingly and the two forms begin to overlap. Initially, only part of one of the submit buttons is obscured, but as the viewport gets continually narrower the effects become more pronounced and eventually the entire button is covered and becomes unclickable. This is a very severe failure as the obscured button controls the primary functionality of the web page, essentially rendering the page unusable on devices where the failure is at its worst.

Given that the failure manifests on a large number of viewport widths and is located near the top of the page, it should be easily detected by a manual tester, which makes it all the more interesting to see the fault manifesting in the live site, available [here](http://midwaymeetup.com).

At 1280px, the page looks like this and all is okay:
![1280px](assets/good-bad/rlf2/1280.png){: .center-image}

At 1024px, the forms have begun to overlap but all functionality is still preserved:
![1024px](assets/good-bad/rlf2/1024.png){: .center-image}

At 768px, the failure is at its most pronounced and the web page is rendered useless:
![768px](assets/good-bad/rlf2/768.png){: .center-image}
