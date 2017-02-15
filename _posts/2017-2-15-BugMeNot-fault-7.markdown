---
layout: post
title: "BugMeNot Fault 7"
---
| **Report Type** | **Distinct RLF No.** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 28 | 456px-514px | TP | Search button has wrapped onto a new line. | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/BugMeNot/fault7/wrappingWidth485.png){: .center-image }

## About Distinct RLF 28

The search button wraps onto a new line as the viewport becomes narrow. The developer should use fluid widths on the main search bar to ensure there is still enough room for the label, form box and button to be shown on a single line. The issue manifests on many common mobile device viewport widths, so a good manual testing procedure should be able to detect it with relative ease.

Here is the failure manifesting:
![Bad]({{ site.baseurl }}/assets/good-bad/rlf28/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK]({{ site.baseurl }}/assets/good-bad/rlf28/ok.png){: .center-image}
