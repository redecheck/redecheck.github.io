---
layout: post
title: "BugMeNot Failure 4"
permalink: BugMeNot-failure-4
---
Below is a summary of the failure report produced by the tool. If it has been classified as a *true positive (TP)*, then further information about the distinct responsive layout failure is available if you scroll down the page.

| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Protrusion| 9 | 403px-678px | TP | Form is clearly protruding out of the page's header. | 

![Screenshot of the fault](assets/images/BugMeNot/fault4/overflow-Width540.png){: .center-image }

## About Distinct RLF 9 {#About-drlf}

The search bar doesn’t resize fluidly as the viewport narrows and the header becomes too small to fit both the logo and the search bar side-by-side. This causes the search bar to overflow the header. To remedy the fault, the developer should either use fluid sizing on the search bar when the viewport is narrow to make sure there is always enough room, or use a media query to adjust the layout of the two elements in relation to one other. The failure manifests for a large number of viewport widths, so should be fairly easy to detect using a manual approach.

Here is the form overflowing the header:
![Bad](assets/good-bad/rlf9/bad.png){: .center-image}

Once the viewport is wide enough, the form can correctly fit inside the header:
![OK](assets/good-bad/rlf9/ok.png){: .center-image}
