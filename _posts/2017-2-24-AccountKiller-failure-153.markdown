---
layout: post
title: "AccountKiller Failure 153"
permalink: AccountKiller-failure-153
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 24 | 394px-459px | TP | Tweet icon clearly wrapped onto a new row | 

![Screenshot of the fault](../assets/images/AccountKiller/fault153/wrappingWidth426.png){: .center-image }

## About Distinct RLF 24 {#About-drlf}

‘Tweet’ icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row. As the viewport continues to narrow, more elements wrap onto the second line which improves the layout a little, but a media query to switch the layout prior to the wrapping behaviour would likely be considered better RWD.

Here is the failure manifesting:
![Bad](../assets/good-bad/rlf24/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](../assets/good-bad/rlf24/ok.png){: .center-image}
