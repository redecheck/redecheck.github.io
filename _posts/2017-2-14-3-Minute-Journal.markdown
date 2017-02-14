---
layout: post
title: "3-Minute-Journal"
elements: 79
decs: 3354
fullurl: www.3minutejournal.com
---

## Distinct RLFs

| RLF No. | Type | Description | Screenshot (Bad) | Screenshot (OK) |
| 1 | Viewport Protrusion | Graph protrudes outside viewport. As the graph has a fixed width and the developer wants to render it side-by-side with the main text, the graph should either have a fluid width or a media query should change the alignment of the elements before the failure occurs (e.g. render the graph below the text). As the failure manifests for around 150px and is viewable at the common viewport width of 1024px, a reasonable manual testing approach should be able to detect it.| [Bad]({{ site.baseurl }}/assets/good-bad/rlf1/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf1/ok.png) |
| 2 | Viewport Protrusion | Graph protrudes outside viewport again, this time at narrow widths. Given the graph is already below the text, the only option to the developer is to implement a fluid width for the element to stop it protruding from the viewport. As it manifests at many viewport widths including several common mobile resolutions, it should be easy to detect manually. | [Bad]({{ site.baseurl }}/assets/good-bad/rlf2/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf2/ok.png) |

Neither failure has currently been addressed by the developers of the site, as can be observed [here](http://3minutejournal.com).

## Full Results

| Report No. | Report Type | Distinct RLF No. | Viewport Range | Classification | Reason | Screenshot |
| 1 | Viewport Protrusion| 2| 320px-371px | TP | 'Feb' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault1/viewportOverflowWidth345.png) |
| 2 | Viewport Protrusion| 2| 320px-583px | TP | 'July' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault2/viewportOverflowWidth451.png) |
| 3 | Viewport Protrusion| 1| 992px-1136px | TP | 'July' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault3/viewportOverflowWidth1064.png) |
| 4 | Viewport Protrusion| 2| 320px-413px | TP | 'Mar' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault4/viewportOverflowWidth366.png) |
| 5 | Viewport Protrusion| 2| 320px-437px | TP | 'Apr' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault5/viewportOverflowWidth378.png) |
| 6 | Viewport Protrusion| 2| 320px-542px | TP | 'Jun' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault6/viewportOverflowWidth431.png) |
| 7 | Viewport Protrusion| 1| 992px-1055px | TP | 'Jun' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault7/viewportOverflowWidth1023.png) |
| 8 | Viewport Protrusion| 2| 320px-499px | TP | 'May' label outside the viewport | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault8/viewportOverflowWidth409.png) |
| 9 | Element Collision| | 320px-767px | NOI | No overlap of content, just DOM coordinates | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault9/overlapWidth543.png) |
| 10 | Element Protrusion| | 438px-449px | NOI | Element is not visibly protruding | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault10/overflow-Width443.png) |
| 11 | Element Protrusion| | 992px-1199px | NOI | Element is not visibly protruding | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault11/overflow-Width1095.png) |
| 12 | Small-Range| | 764px-767px | FP | No significant layout change, just coincidental labelling | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault12/smallrangeWidth765.png) |
