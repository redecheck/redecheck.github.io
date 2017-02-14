---
layout: post
title: "BugMeNot"
elements: 41
decs: 237
fullurl: bugmenot.com
---

# Distinct RLFs

| RLF No. | Type | Description | Screenshot (Bad) | Screenshot (OK) |
| 8 | Element Protrusion | The search bar doesn't resize fluidly as the viewport narrows and the header becomes too small to fit both the logo and the search bar side-by-side. This causes the search bar to overflow the header. To remedy the fault, the developer should either use fluid sizing on the search bar when the viewport is narrow to make sure there is always enough room, or use a media query to adjust the layout of the two elements in relation to one other. The failure manifests for a large number of viewport widths, so should be fairly easy to detect using a manual approach. | [Bad]({{ site.baseurl }}/assets/good-bad/rlf8/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf8/ok.png) |
| 9 | Wrapping | The search button wraps onto a new line as the viewport becomes narrow. The developer should use fluid widths on the main search bar to ensure there is still enough room for the label, form box and button to be shown on a single line. The issue manifests on many common mobile device viewport widths, so a good manual testing procedure should be able to detect it with relative ease. | [Bad]({{ site.baseurl }}/assets/good-bad/rlf9/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf9/ok.png) |
| 10 |
| 11 |

## Full Results

| Report No. | Report Type | Distinct RLF No. | Viewport Range | Classification | Reason | Screenshot |
| 180 | Viewport Protrusion| | 320px-353px | TP | Part of input box obscured by viewport protrusion, so a TP | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault1/viewportOverflowWidth336.png) |
| 181 | Viewport Protrusion| | 320px-340px | TP | Part of input box obscured by viewport protrusion, so a TP | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault2/viewportOverflowWidth330.png) |
| 182 | Element Protrusion| | 335px-529px | NOI | Element is not visibly protruding | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault3/overflow-Width432.png) |
| 183 | Element Protrusion| | 403px-678px | TP | Form is clearly protruding out of the page's header. | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault4/overflow-Width540.png) |
| 184 | Element Protrusion| | 320px-420px | NOI | Element is not visibly protruding | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault5/overflow-Width370.png) |
| 185 | Element Protrusion| | 320px-334px | NOI | Element is not visibly protruding | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault6/overflow-Width327.png) |
| 186 | Wrapping| | 456px-514px | TP | Search button has wrapped onto a new line. | [Click]({{ site.baseurl }}/assets/images/BugMeNot/fault7/wrappingWidth485.png) |
