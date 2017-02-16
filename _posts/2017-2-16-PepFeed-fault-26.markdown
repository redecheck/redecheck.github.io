---
layout: post
title: "PepFeed Fault 26"
---
| **Report Type** | **Distinct RLF No.** | **Viewport Range** | **Classification** | **Reason** |
| Small-Range| 6 | 415px-415px | TP | Layout only true for 415px, so a TP. | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/PepFeed/fault26/smallrangeWidth415.png){: .center-image }

## About Distinct RLF 6

When the viewport is wide enough, three content panels are rendered side by side and at very narrow widths they are stacked into a single column. However, in between these widths two of the panels overlap, obscuring some of the content. As the failure occurs at the top of the page, it makes the page look very unprofessional and has the potential to discourage visitors from using the service provided.

Given that the failure manifests at a single viewport width, it would be likely undetected by a manual tester, despite being located near the top of the page. Therefore, it comes as little surprise the fault is still manifesting in the live site, available [here](http://pepfeed.com).

At very narrow widths, the page looks like this and all is okay:
![400px]({{ site.baseurl }}/assets/good-bad/rlf6/400.png){: .center-image}

At 415px, the panels 2 and 3 are overlapping:
![415px]({{ site.baseurl }}/assets/good-bad/rlf6/415.png){: .center-image}

At 420px, the panels are no longer overlapping:
![420px]({{ site.baseurl }}/assets/good-bad/rlf6/420.png){: .center-image}
