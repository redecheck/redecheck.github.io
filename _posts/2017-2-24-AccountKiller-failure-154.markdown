---
layout: post
title: "AccountKiller Failure 154"
permalink: AccountKiller-failure-154
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Wrapping| 25 | 808px-959px | TP | 'The Atlantic' clearly wrapped onto a new row | 

![Screenshot of the fault](../assets/images/AccountKiller/fault154/wrappingWidth883.png){: .center-image }

## About Distinct RLF 25 {#About-drlf}

‘The Atlantic’ wraps onto a new line. No impact on functionality, but aesthetically, two rows of three icons might look much more professional. Eventually the elements all wrap so they are in 2 rows of 3 and then 3 rows of 2, but a developer should probably use media queries to implement this rather than relying on the incongruously wrapping of the elements. The failure manifests at a decent number of viewport widths, but due to its fairly subtle aesthetics and the fact its located near the bottom of the page, it would likely be undetected by a manual tester.

Here is the failure manifesting:
![Bad](../assets/good-bad/rlf25/bad.png){: .center-image}

Here is the page once the viewport is wide enough to show all elements in a single row:
![OK](../assets/good-bad/rlf25/ok.png){: .center-image}
