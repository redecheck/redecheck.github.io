---
layout: page
title: Results Archive
permalink: /results-archive/
---

### Navigating around the Archive
Exploring the results archive is straight-forward. The individual failure reports are listed below, separated into three different categories. The first, TP (True Positive), are failures highlighting actual visual issues with the layout of the site, such as overlapping elements, elements overflowing their parent or the viewport, or wrapping elements. The second, FP (False Positive) are reported failures which are actually layout behaviour intended by the developer. Finally, NOI (Non-Observable Issues) are failures that are not visible to the user but present potential future issues at the DOM level.

The failure reports are also ordered by type; *Element Collision*, *Element Protrusion*, *Viewport Protrusion*, *Small-Range* and finally, *Wrapping*. The main table provides an overview of the failure, such the web page it occurred on and its classification. For more detailed information and the screenshot produces by the tool, click on the link for the relevant failure report.

### Understanding the Failure Reports

The different failure types are highlighted in different ways to make them as easy to understand as possible. The following table will explain how to interpret the screenshots, followed by several examples:

| **Failure Type** | **Interpretation** | **Example** |
| Element Collision | The two offending elements will be highlighted with red and blue boxes, respectively. In the example on the right, the panels numbered 1 and 2 are clearly shown to be overlapping| ![Click](../assets/examples/overlap.png){: .table-image} |
| Element Protrusion | The protruding element will be highlighted in blue, with the ancestor it is currently overlapping with (signifying the protrusion) highlighted in red. The example shows a set of "invisible" navigation links (blue) which have protruded outside of the header bar (red).  |  ![Click](../assets/examples/overflow.png){: .center-image}{: .table-image} |
| Viewport Protrusion | The viewport window will be highlighted in green, while the element protruding outside of the viewport will be highlighted in red. The example image shows a carousel bar (red) protruding outside of the viewport window (green). |  ![Click](../assets/examples/viewport-protrusion.png){: .table-image} |
| Small-Range | The two elements whose layout is only true for a small range of viewport widths will again be highlighted in red and blue boxes. The example shows the header bar and main content banner in a peculiar alignment for the single viewport width of 980px.| ![Click](../assets/examples/small-range.png){: .table-image} |
| Wrapping | The "wrapped" element will be highlighted in red, while the elements in the row it has wrapped from will be highlighted in blue. The example shows the search button (red) wrapping onto a new row from the label and input box (blue).| ![Click](../assets/examples/wrapping.png){: .table-image} |

<a href="#TP">Jump to True Positives</a>

<a href="#FP">Jump to False Positives</a>

<a href="#NOI">Jump to Non-Observable Issues</a>



### True Positives### {#TP}

| Report Type | Distinct RLF | Web Page | Viewport Range | Classification | Reason |
| Element Collision| 1 | CloudConvert | 980px-980px | TP | Header and main content panel clearly overlapping, obscuring the banner [Screenshot and Detailed Information](../2017/02/20/CloudConvert-failure-1.html) |
| Element Collision| 2 | MidwayMeetup | 768px-1132px | TP | Form is clearly overlapping with the main panel, and button is unclickable [Screenshot and Detailed Information](../2017/02/20/MidwayMeetup-failure-2.html) |
| Element Collision| 3 | PepFeed | 415px-546px | TP | Panels 1 and 2 clearly overlapping [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-4.html) |
| Element Collision| 4 | PepFeed | 547px-700px | TP | Panels 1 and 3 clearly overlapping [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-8.html) |
| Element Collision| 5 | PepFeed | 769px-933px | TP | Panels 1 and 3 clearly overlapping [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-9.html) |
| Element Collision| 6 | PepFeed | 415px-415px | TP | Panels 2 and 3 clearly overlapping [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-10.html) |
| Element Collision| 7 | StumbleUpon | 320px-439px | TP | Element collision clearly causing undesirable layout [Screenshot and Detailed Information](../2017/02/20/StumbleUpon-failure-1.html) |
| Element Collision| 8 | WillMyPhoneWork | 990px-991px | TP | Header and main content clearly overlapping [Screenshot and Detailed Information](../2017/02/20/WillMyPhoneWork-failure-1.html) |
| Element Protrusion| 9 | BugMeNot | 403px-678px | TP | Form is clearly protruding out of the page's header. [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-4.html) |
| Element Protrusion| 10 | Consumer-Reports | 392px-767px | TP | Text has clearly protruding outside its container [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-14.html) |
| Element Protrusion| 11 | Pdf-Escape | 801px-805px | TP | Navigation links have clearly protruded outside the navbar and become invisible and unclickable [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-8.html) |
| Viewport Protrusion| 12 | 3-Minute-Journal | 320px-371px | TP | 'Feb' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-1.html) |
| Viewport Protrusion| 12 | 3-Minute-Journal | 320px-583px | TP | 'July' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-2.html) |
| Viewport Protrusion| 13 | 3-Minute-Journal | 992px-1136px | TP | 'July' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-3.html) |
| Viewport Protrusion| 12 | 3-Minute-Journal | 320px-413px | TP | 'Mar' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-4.html) |
| Viewport Protrusion| 12 | 3-Minute-Journal | 320px-437px | TP | 'Apr' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-5.html) |
| Viewport Protrusion| 12 | 3-Minute-Journal | 320px-542px | TP | 'Jun' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-6.html) |
| Viewport Protrusion| 13 | 3-Minute-Journal | 992px-1055px | TP | 'Jun' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-7.html) |
| Viewport Protrusion| 12 | 3-Minute-Journal | 320px-499px | TP | 'May' label outside the viewport [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-8.html) |
| Viewport Protrusion| 14 | BugMeNot | 320px-353px | TP | Part of input box obscured by viewport protrusion, so a TP [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-1.html) |
| Viewport Protrusion| 15 | BugMeNot | 320px-340px | TP | Part of input box obscured by viewport protrusion, so a TP [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-2.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-365px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-4.html) |
| Viewport Protrusion| 17 | Consumer-Reports | 1025px-1110px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-5.html) |
| Viewport Protrusion| 18 | Consumer-Reports | 768px-1039px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-6.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-377px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-7.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-375px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-8.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-377px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-9.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-377px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-10.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-375px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-11.html) |
| Viewport Protrusion| 16 | Consumer-Reports | 320px-375px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-12.html) |
| Viewport Protrusion| 19 | Duolingo | 981px-1099px | TP | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-1.html) |
| Viewport Protrusion| 19 | Duolingo | 981px-1099px | TP | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-3.html) |
| Viewport Protrusion| 20 | HotelWifiTest | 415px-767px | TP | Main container clearly protruding from the viewport, obscuring lots of content [Screenshot and Detailed Information](../2017/02/20/HotelWifiTest-failure-1.html) |
| Viewport Protrusion| 21 | Pdf-Escape | 768px-850px | TP | Part of image obscured by protrusion outside viewport [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-4.html) |
| Viewport Protrusion| 22 | PepFeed | 415px-768px | TP | Amazon logo obscured by viewport at narrower width than screenshot. [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-1.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-1.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-2.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-3.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-4.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-5.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-6.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-7.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-8.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-9.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-10.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-11.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-12.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-13.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-14.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-15.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-16.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-17.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-18.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-19.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-20.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-21.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-22.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-23.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-24.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-25.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-26.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-27.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-28.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-29.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-30.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-31.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-32.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-33.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-34.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-35.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-36.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-37.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-38.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-39.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-40.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-41.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-42.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-43.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-44.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-45.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-46.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-47.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-48.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-49.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-50.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-51.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-52.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-54.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-55.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-56.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-57.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-58.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-59.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-61.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-62.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-63.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-64.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-65.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-66.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-67.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-68.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-70.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-71.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-72.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-73.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-74.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-75.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-76.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-77.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-78.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-79.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-80.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-81.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-82.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-83.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-84.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-85.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-86.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-87.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-88.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-89.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-90.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-91.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-92.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-93.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-94.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-95.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-96.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-97.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-98.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-99.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-100.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-101.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-102.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-103.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-104.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-105.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-106.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-107.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-108.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-109.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-110.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-111.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-112.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-113.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-114.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-115.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-116.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-117.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-118.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-119.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-120.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-121.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-123.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-124.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-125.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-126.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-127.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-128.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-129.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-130.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-131.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-132.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-133.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-134.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-135.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-136.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-137.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-138.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-139.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-140.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-141.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-142.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-143.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-145.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-146.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-147.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-148.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-149.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-150.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-151.html) |
| Small-Range| 23 | AccountKiller | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-152.html) |
| Small-Range| 1 | CloudConvert | 980px-980px | TP | Layout only true at 980px, so clearly a TP. [Screenshot and Detailed Information](../2017/02/20/CloudConvert-failure-2.html) |
| Small-Range| 6 | PepFeed | 415px-415px | TP | Layout only true for 415px, so a TP. [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-24.html) |
| Small-Range| 6 | PepFeed | 415px-415px | TP | Layout only true for 415px, so a TP. [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-26.html) |
| Small-Range| 8 | WillMyPhoneWork | 990px-991px | TP | Elements are only overlapping for a couple of widths, so a TP [Screenshot and Detailed Information](../2017/02/20/WillMyPhoneWork-failure-3.html) |
| Small-Range| 8 | WillMyPhoneWork | 990px-991px | TP | Alignment only true for a couple of widths, so a TP [Screenshot and Detailed Information](../2017/02/20/WillMyPhoneWork-failure-4.html) |
| Wrapping| 24 | AccountKiller | 394px-459px | TP | Tweet icon clearly wrapped onto a new row [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-153.html) |
| Wrapping| 25 | AccountKiller | 808px-959px | TP | 'The Atlantic' clearly wrapped onto a new row [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-154.html) |
| Wrapping| 26 | AirBnb | 321px-335px | TP | 'Terms and Privacy' clearly wrapped onto new row [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-12.html) |
| Wrapping| 27 | AirBnb | 326px-356px | TP | Instagram logo clearly wrapped onto new row [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-13.html) |
| Wrapping| 28 | BugMeNot | 456px-514px | TP | Search button has wrapped onto a new line. [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-7.html) |
| Wrapping| 29 | Covered-Calendar | 320px-385px | TP | 'Privacy Policy' cleared wraps onto a new line [Screenshot and Detailed Information](../2017/02/20/Covered-Calendar-failure-4.html) |
| Wrapping| 30 | Covered-Calendar | 768px-979px | TP | Header navigation link clearly wraps onto a new line [Screenshot and Detailed Information](../2017/02/20/Covered-Calendar-failure-5.html) |
| Wrapping| 31 | Ninite | 347px-395px | TP | 'terms' nav link clearly wrapped onto new line [Screenshot and Detailed Information](../2017/02/20/Ninite-failure-2.html) |
| Wrapping| 32 | PepFeed | 320px-386px | TP | 'The Verge' has clearly wrapped onto a new line [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-28.html) |
| Wrapping| 33 | UserSearch | 625px-794px | TP | Final navigation link clearly wrapped onto a new line [Screenshot and Detailed Information](../2017/02/20/UserSearch-failure-2.html) |

### False Positives### {#FP}

| Report Type | Distinct RLF | Web Page | Viewport Range | Classification | Reason |
| Small-Range|  | 3-Minute-Journal | 764px-767px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-12.html) |
| Small-Range|  | AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-53.html) |
| Small-Range|  | AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-60.html) |
| Small-Range|  | AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-69.html) |
| Small-Range|  | AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-122.html) |
| Small-Range|  | AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/AccountKiller-failure-144.html) |
| Small-Range|  | AirBnb | 1199px-1199px | FP | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-10.html) |
| Small-Range|  | AirBnb | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-11.html) |
| Small-Range|  | Consumer-Reports | 768px-770px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-24.html) |
| Small-Range|  | Duolingo | 378px-380px | FP | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-6.html) |
| Small-Range| null | Honey | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/Honey-failure-11.html) |
| Small-Range| null | Honey | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/Honey-failure-12.html) |
| Small-Range| null | Honey | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/Honey-failure-13.html) |
| Small-Range|  | HotelWifiTest | 992px-992px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../2017/02/20/HotelWifiTest-failure-2.html) |
| Small-Range|  | HotelWifiTest | 769px-769px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../2017/02/20/HotelWifiTest-failure-3.html) |
| Small-Range| null | Mailinator | 499px-502px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../2017/02/20/Mailinator-failure-2.html) |
| Small-Range| null | Mailinator | 499px-502px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../2017/02/20/Mailinator-failure-3.html) |
| Small-Range|  | PepFeed | 480px-480px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-12.html) |
| Small-Range|  | PepFeed | 732px-736px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-13.html) |
| Small-Range|  | PepFeed | 598px-600px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-14.html) |
| Small-Range|  | PepFeed | 748px-750px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-15.html) |
| Small-Range|  | PepFeed | 1024px-1024px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-16.html) |
| Small-Range|  | PepFeed | 992px-993px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-17.html) |
| Small-Range|  | PepFeed | 965px-965px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-18.html) |
| Small-Range|  | PepFeed | 480px-480px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-19.html) |
| Small-Range|  | PepFeed | 748px-750px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-20.html) |
| Small-Range|  | PepFeed | 598px-600px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-21.html) |
| Small-Range|  | PepFeed | 732px-736px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-22.html) |
| Small-Range|  | PepFeed | 769px-773px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-23.html) |
| Small-Range|  | PepFeed | 1200px-1202px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-25.html) |
| Small-Range|  | PepFeed | 992px-993px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-27.html) |
| Small-Range| null | Pocket | 768px-770px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-6.html) |
| Small-Range| null | Pocket | 768px-768px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-7.html) |
| Small-Range| null | Pocket | 768px-770px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-8.html) |
| Small-Range| null | RunPee | 479px-479px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/RunPee-failure-1.html) |
| Small-Range| null | RunPee | 480px-483px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/RunPee-failure-2.html) |
| Small-Range| null | RunPee | 480px-480px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/RunPee-failure-3.html) |
| Small-Range| null | RunPee | 481px-481px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/RunPee-failure-4.html) |
| Small-Range| null | RunPee | 768px-772px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/RunPee-failure-5.html) |
| Small-Range| null | TopDocumentary | 689px-691px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-12.html) |
| Small-Range| null | TopDocumentary | 593px-596px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-13.html) |
| Small-Range| null | ZeroDollarMovies | 481px-483px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/ZeroDollarMovies-failure-1.html) |
| Small-Range| null | ZeroDollarMovies | 481px-481px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../2017/02/20/ZeroDollarMovies-failure-2.html) |
| Wrapping|  | Duolingo | 378px-399px | FP | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-7.html) |
| Wrapping|  | Duolingo | 830px-881px | FP | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-8.html) |
| Wrapping|  | Ninite | 410px-614px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../2017/02/20/Ninite-failure-1.html) |
| Wrapping| null | RunPee | 480px-681px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../2017/02/20/RunPee-failure-6.html) |
| Wrapping|  | StumbleUpon | 661px-840px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../2017/02/20/StumbleUpon-failure-2.html) |

### Non-Observable Issues### {#NOI}

| Report Type | Distinct RLF | Web Page | Viewport Range | Classification | Reason |
| Element Collision|  | 3-Minute-Journal | 320px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-9.html) |
| Element Collision|  | AirBnb | 744px-1127px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-5.html) |
| Element Collision|  | Consumer-Reports | 336px-767px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-15.html) |
| Element Collision|  | Consumer-Reports | 320px-384px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-16.html) |
| Element Collision|  | Consumer-Reports | 648px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-18.html) |
| Element Collision|  | Consumer-Reports | 320px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-20.html) |
| Element Collision|  | Consumer-Reports | 691px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-21.html) |
| Element Collision|  | Consumer-Reports | 329px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-22.html) |
| Element Collision|  | Consumer-Reports | 320px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-23.html) |
| Element Collision|  | Duolingo | 320px-980px | NOI | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-5.html) |
| Element Collision| null | Mailinator | 992px-1199px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Mailinator-failure-1.html) |
| Element Collision|  | PepFeed | 415px-479px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-5.html) |
| Element Collision|  | PepFeed | 320px-479px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-6.html) |
| Element Collision|  | PepFeed | 934px-965px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-11.html) |
| Element Collision| null | Pocket | 487px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-1.html) |
| Element Collision| null | Pocket | 487px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-2.html) |
| Element Collision| null | TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-1.html) |
| Element Collision| null | TopDocumentary | 765px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-2.html) |
| Element Collision| null | TopDocumentary | 682px-688px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-5.html) |
| Element Collision| null | TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-6.html) |
| Element Collision| null | TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-8.html) |
| Element Collision| null | TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-9.html) |
| Element Collision| null | TopDocumentary | 681px-688px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-10.html) |
| Element Collision|  | UserSearch | 802px-897px | NOI | No visible content overlap, just DOM coordinates [Screenshot and Detailed Information](../2017/02/20/UserSearch-failure-1.html) |
| Element Protrusion|  | 3-Minute-Journal | 438px-449px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-10.html) |
| Element Protrusion|  | 3-Minute-Journal | 992px-1199px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/3-Minute-Journal-failure-11.html) |
| Element Protrusion|  | AirBnb | 320px-743px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-6.html) |
| Element Protrusion|  | AirBnb | 320px-743px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-7.html) |
| Element Protrusion|  | AirBnb | 744px-768px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-8.html) |
| Element Protrusion|  | AirBnb | 320px-743px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-9.html) |
| Element Protrusion|  | BugMeNot | 335px-529px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-3.html) |
| Element Protrusion|  | BugMeNot | 320px-420px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-5.html) |
| Element Protrusion|  | BugMeNot | 320px-334px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/BugMeNot-failure-6.html) |
| Element Protrusion|  | Consumer-Reports | 771px-1180px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-13.html) |
| Element Protrusion|  | Consumer-Reports | 771px-1180px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-17.html) |
| Element Protrusion|  | Consumer-Reports | 320px-767px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-19.html) |
| Element Protrusion| null | Honey | 1200px-1200px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-3.html) |
| Element Protrusion| null | Honey | 1001px-1199px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-4.html) |
| Element Protrusion| null | Honey | 320px-1199px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-5.html) |
| Element Protrusion| null | Honey | 1200px-1200px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-6.html) |
| Element Protrusion| null | Honey | 320px-325px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-7.html) |
| Element Protrusion| null | Honey | 566px-767px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-8.html) |
| Element Protrusion| null | Honey | 682px-767px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-9.html) |
| Element Protrusion| null | Honey | 320px-325px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Honey-failure-10.html) |
| Element Protrusion|  | MidwayMeetup | 768px-1024px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/MidwayMeetup-failure-3.html) |
| Element Protrusion|  | Pdf-Escape | 843px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-5.html) |
| Element Protrusion|  | Pdf-Escape | 768px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-6.html) |
| Element Protrusion|  | Pdf-Escape | 768px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-7.html) |
| Element Protrusion|  | Pdf-Escape | 320px-479px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-9.html) |
| Element Protrusion|  | Pdf-Escape | 768px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-10.html) |
| Element Protrusion|  | PepFeed | 768px-991px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-3.html) |
| Element Protrusion|  | PepFeed | 768px-991px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-7.html) |
| Element Protrusion| null | Pocket | 768px-900px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-3.html) |
| Element Protrusion| null | Pocket | 877px-885px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-4.html) |
| Element Protrusion| null | Pocket | 877px-885px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/Pocket-failure-5.html) |
| Element Protrusion| null | TopDocumentary | 509px-512px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-3.html) |
| Element Protrusion| null | TopDocumentary | 566px-944px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-4.html) |
| Element Protrusion| null | TopDocumentary | 549px-944px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-7.html) |
| Element Protrusion| null | TopDocumentary | 558px-944px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../2017/02/20/TopDocumentary-failure-11.html) |
| Element Protrusion|  | WillMyPhoneWork | 992px-1199px | NOI | Element is not visibly protruding from its parent [Screenshot and Detailed Information](../2017/02/20/WillMyPhoneWork-failure-2.html) |
| Viewport Protrusion|  | AirBnb | 320px-743px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-1.html) |
| Viewport Protrusion|  | AirBnb | 320px-743px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-2.html) |
| Viewport Protrusion|  | AirBnb | 320px-710px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-3.html) |
| Viewport Protrusion|  | AirBnb | 744px-1073px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/AirBnb-failure-4.html) |
| Viewport Protrusion|  | Consumer-Reports | 768px-782px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-1.html) |
| Viewport Protrusion|  | Consumer-Reports | 1200px-1400px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-2.html) |
| Viewport Protrusion|  | Consumer-Reports | 768px-782px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/Consumer-Reports-failure-3.html) |
| Viewport Protrusion|  | Covered-Calendar | 1200px-1240px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/Covered-Calendar-failure-1.html) |
| Viewport Protrusion|  | Covered-Calendar | 1200px-1240px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/Covered-Calendar-failure-2.html) |
| Viewport Protrusion|  | Covered-Calendar | 1200px-1240px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/Covered-Calendar-failure-3.html) |
| Viewport Protrusion| null | Days-Old | 320px-340px | NOI | No visible protrusion outside the viewport [Screenshot and Detailed Information](../2017/02/20/Days-Old-failure-1.html) |
| Viewport Protrusion| null | Dictation | 320px-480px | NOI | No visible protrusion outside the viewport [Screenshot and Detailed Information](../2017/02/20/Dictation-failure-1.html) |
| Viewport Protrusion|  | Duolingo | 981px-1276px | NOI | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-2.html) |
| Viewport Protrusion|  | Duolingo | 981px-1267px | NOI | null [Screenshot and Detailed Information](../2017/02/20/Duolingo-failure-4.html) |
| Viewport Protrusion| null | Honey | 768px-789px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/Honey-failure-1.html) |
| Viewport Protrusion| null | Honey | 992px-1009px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/Honey-failure-2.html) |
| Viewport Protrusion|  | MidwayMeetup | 320px-535px | NOI | No visible protrusion of element outside the viewport [Screenshot and Detailed Information](../2017/02/20/MidwayMeetup-failure-1.html) |
| Viewport Protrusion|  | Pdf-Escape | 320px-800px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-1.html) |
| Viewport Protrusion|  | Pdf-Escape | 768px-780px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-2.html) |
| Viewport Protrusion|  | Pdf-Escape | 960px-972px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/Pdf-Escape-failure-3.html) |
| Viewport Protrusion|  | PepFeed | 1025px-1080px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../2017/02/20/PepFeed-failure-2.html) |
| Viewport Protrusion| null | WhatShouldIReadNext | 601px-611px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/WhatShouldIReadNext-failure-1.html) |
| Viewport Protrusion| null | WhatShouldIReadNext | 601px-611px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../2017/02/20/WhatShouldIReadNext-failure-2.html) |
