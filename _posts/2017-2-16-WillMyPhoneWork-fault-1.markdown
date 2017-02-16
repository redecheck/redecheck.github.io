---
layout: post
title: "WillMyPhoneWork Fault 1"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 8 | 990px-991px | TP | Header and main content clearly overlapping | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/WillMyPhoneWork/fault1/overlapWidth990.png){: .center-image }

## About Distinct RLF 8

At the viewport widths of 990px and 991px, a misuse of media queries controlling the switch between the mobile and desktop versions of the site results in the header bar and the main content banner overlapping. Given the failure occurs right at the top of the web page, it could be said to be fairly serious, as it could make visitors to the site unsure of the site's quality and by extension, the quality of the service offered by the site. As it only occurs at two viewport widths, manual testing would be highly unlikely to detect the failure. It still currently manifests in the live site, available [here](http://willmyphonework.net/).

At 989px, the page looks like this:
![989px]({{ site.baseurl }}/assets/good-bad/rlf8/989.png){: .center-image}

At 990px, the page looks like this:
![980px]({{ site.baseurl }}/assets/good-bad/rlf8/990.png){: .center-image}

At 992px, the page looks like this:
![992px]({{ site.baseurl }}/assets/good-bad/rlf8/992.png){: .center-image}
