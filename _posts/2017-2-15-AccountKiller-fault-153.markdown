---
layout: post
title: "AccountKiller Fault 153"
---
| **Report Type** | **Distinct RLF No.** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 24 | 394px-459px | TP | Tweet icon clearly wrapped onto a new row | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/AccountKiller/fault153/wrappingWidth426.png){: .center-image }

## About Distinct RLF 24

‘Tweet’ icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row. As the viewport continues to narrow, more elements wrap onto the second line which improves the layout a little, but a media query to switch the layout prior to the wrapping behaviour would likely be considered better RWD.

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf24/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf24/ok.png){: .center-image}
