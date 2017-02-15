---
layout: post
title: "AirBnb Fault 12"
---
| **Report Type** | **Distinct RLF No.** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 26 | 321px-335px | TP | 'Terms and Privacy' clearly wrapped onto new row | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/AirBnb/fault12/wrappingWidth328.png){: .center-image }

## About Distinct RLF 26

‘Terms & Privacy’ icon wraps onto a new line. Not a major issue at all, but something the developer may want to remedy. It is only visible for a few viewport widths and is also located in the footer of a long web page, so manual testing would likely find it difficult to detect. An update to the [live version](http://airbnb.com) of the page means this failure no longer manifests.

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf26/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf26/ok.png){: .center-image}
