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

| Failure No. | Category | Screenshot | Classification | Reason | Distinct RLF |
| 1| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault1/viewportOverflowWidth345.png) | TP | 'Feb' label outside the viewport | 1|
| 2| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault2/viewportOverflowWidth451.png) | TP | 'July' label outside the viewport | 1|
| 3| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault3/viewportOverflowWidth1064.png) | TP | 'July' label outside the viewport | 2|
| 4| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault4/viewportOverflowWidth366.png) | TP | 'Mar' label outside the viewport | 1|
| 5| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault5/viewportOverflowWidth378.png)| TP | 'Apr' label outside the viewport | 1|
| 6| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault6/viewportOverflowWidth431.png) | TP | 'Jun' label outside the viewport | 1|
| 7| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault7/viewportOverflowWidth1023.png) | TP | 'Jun' label outside the viewport | 2|
| 8| Viewport Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault8/viewportOverflowWidth409.png) | TP | 'May' label outside the viewport | 1|
| 9| Element Collision | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault9/overlapWidth543.png) | NOI | No overlap of content, just DOM coordinates | |
| 10| Element Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault10/overflow-Width443.png) | NOI | Element is not visibly protruding | |
| 11| Element Protrusion | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault11/overflow-Width1095.png) | NOI | Element is not visibly protruding | |
| 12| Small-Range | [Click]({{ site.baseurl }}/assets/images/3-Minute-Journal/fault12/smallrangeWidth765.png) | FP | No significant layout change, just coincidental labelling | |
