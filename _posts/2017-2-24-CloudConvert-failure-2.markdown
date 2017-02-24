---
layout: post
title: "CloudConvert Failure 2"
permalink: CloudConvert-failure-2
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Small-Range| 1 | 980px-980px | TP | Layout only true at 980px, so clearly a TP. | 

![Screenshot of the fault](../assets/images/CloudConvert/fault2/smallrangeWidth980.png){: .center-image }

## About Distinct RLF 1 {#About-drlf}

At the single viewport width of 980px, a misuse of media queries controlling the switch between the mobile and desktop versions of the site results in the header bar and the main content banner overlapping. Given the failure occurs right at the top of the web page, it could be said to be fairly serious, as it could make visitors to the site unsure of the site's quality and by extension, the quality of the service offered by the site. As it only occurs at a single viewport width, manual testing would be highly unlikely to detect the failure. It still currently manifests in the live site, available [here](http://cloudconvert.com).

At 979px, the page looks like this:
![979px](../assets/good-bad/rlf1/979.png){: .center-image}

At 980px, the page looks like this:
![980px](../assets/good-bad/rlf1/980.png){: .center-image}

At 981px, the page looks like this:
![981px](../assets/good-bad/rlf1/981.png){: .center-image}
