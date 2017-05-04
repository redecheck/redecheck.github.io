---
layout: post
title: "WillMyPhoneWork Failure 4"
permalink: WillMyPhoneWork-failure-4
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Small-Range| 8 | 990px-991px | TP | Alignment only true for a couple of widths, so a TP | 

![Screenshot of the fault](../assets/images/WillMyPhoneWork/fault4/smallrangeWidth990.png){: .center-image }

## About Distinct RLF 8 {#About-drlf}

At the viewport widths of 990px and 991px, a misuse of media queries controlling the switch between the mobile and desktop versions of the site results in the header bar and the main content banner overlapping. Given the failure occurs right at the top of the web page, it could be said to be fairly serious, as it could make visitors to the site unsure of the site's quality and by extension, the quality of the service offered by the site. As it only occurs at two viewport widths, manual testing would be highly unlikely to detect the failure. It still currently manifests in the live site, available [here](http://willmyphonework.net/).

At 989px, the page looks like this:
![989px](../assets/good-bad/rlf8/989.png){: .center-image}

At 990px, the page looks like this:
![980px](../assets/good-bad/rlf8/990.png){: .center-image}

At 992px, the page looks like this:
![992px](../assets/good-bad/rlf8/992.png){: .center-image}
