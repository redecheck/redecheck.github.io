---
layout: post
title: "PepFeed Failure 4"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 3 | 415px-546px | TP | Panels 1 and 2 clearly overlapping | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/PepFeed/fault4/overlapWidth480.png){: .center-image }

## About Distinct RLF 3

When the viewport is wide enough, three content panels are rendered side by side and at very narrow widths they are stacked into a single column. However, in between these widths two of the panels overlap, obscuring some of the content. As the failure occurs at the top of the page, it makes the page look very unprofessional and has the potential to discourage visitors from using the service provided.

Given that the failure manifests on a reasonable number of viewport widths and is located near the top of the page, it should be easily detected by a manual tester. However, the fault is still manifesting in the live site, available [here](http://pepfeed.com).

At very narrow widths, the page looks like this and all is okay:
![400px]({{ site.baseurl }}/assets/good-bad/rlf3/400.png){: .center-image}

At 750px, the layout is in a row and all is well:
![750px]({{ site.baseurl }}/assets/good-bad/rlf3/750.png){: .center-image}

However, in between these widths, an overlap occurs
![450px]({{ site.baseurl }}/assets/good-bad/rlf3/450.png){: .center-image}

Even after a media query changes the size of the elements, they are still overlapping:
![500px]({{ site.baseurl }}/assets/good-bad/rlf3/500.png){: .center-image}
