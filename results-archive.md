---
layout: page
title: Results Archive
permalink: /results-archive/
---

### Navigating around the Archive
Exploring the results archive is straight-forward. The individual failure reports are listed below, separated into three different categories. The first, TP (True Positive), are failures highlighting actual visual issues with the layout of the site, such as overlapping elements, elements overflowing their parent or the viewport, or wrapping elements. The second, FP (False Positive) are reported failures which are actually layout behaviour intended by the developer. Finally, NOI (Non-Observable Issues) are failures that are not visible to the user but present potential future issues at the DOM level.

The failure reports are first ordered by type; *Element Collision*, *Element Protrusion*, *Viewport Protrusion*, *Small-Range* and finally, *Wrapping*. They are then ordered alphabetically on the "Web Page" column. In a couple of cases, this may cause the "Distinct RLF" table values to appear in a slightly inconsistent order.

When browsing the table, you will notice in some cases multiple failure reports have been linked to the same Distinct RLF number. This was done by the authors manually, grouping together related failures involving common HTML elements that are likely to emanate from a single defect in the HTML and CSS of the web page.

The main table provides an overview of the failure, such as the web page it occurred on and its classification. For more detailed information and the screenshot produced by the tool, click on the link for the relevant failure report labled "Screenshot and Detailed Information". If you would prefer to jump directly to information regarding the distinct layout failure, simply click on the number in the "Distinct RLF" column.

### Understanding the Failure Reports

The different failure types are highlighted in different ways to make them as easy to understand as possible. The following table will explain how to interpret the screenshots, followed by several examples:

| **Failure Type** | **Interpretation** | **Example** |
| Element Collision | The two offending elements will be highlighted with red and blue boxes, respectively. In the example on the right, the panels numbered 1 and 2 are clearly shown to be overlapping| ![Click](../assets/examples/overlap.png){: .table-image} Screenshot from *MidwayMeetup* [More Info](../MidwayMeetup-failure-2.html)|
| Element Protrusion | The protruding element will be highlighted in blue, with the ancestor it is currently overlapping with (signifying the protrusion) highlighted in red. The example shows a set of "invisible" navigation links (blue) which have protruded outside of the header bar (red).  |  ![Click](../assets/examples/overflow.png){: .table-image} Screenshot from *BugMeNot* [More Info](../Pdf-Escape-failure-8.html)|
| Viewport Protrusion | The viewport window will be highlighted in green, while the element protruding outside of the viewport will be highlighted in red. The example image shows a carousel bar (red) protruding outside of the viewport window (green). |  ![Click](../assets/examples/viewport-protrusion.png){: .table-image} Screenshot from *Duolingo* [More Info](../Duolingo-failure-1.html)|
| Small-Range | The two elements whose layout is only true for a small range of viewport widths will again be highlighted in red and blue boxes. The example shows the header bar and main content banner in a peculiar alignment for the single viewport width of 980px.| ![Click](../assets/examples/small-range.png){: .table-image} Screenshot from *CloudConvert* [More Info](../CloudConvert-failure-1.html)|
| Wrapping | The "wrapped" element will be highlighted in red, while the elements in the row it has wrapped from will be highlighted in blue. The example shows the search button (red) wrapping onto a new row from the label and input box (blue).| ![Click](../assets/examples/wrapping.png){: .center-image} Screenshot from *BugMeNot* [More Info](../BugMeNot-failure-7.html) |

<a href="#TP">Jump to True Positives</a>

<a href="#FP">Jump to False Positives</a>

<a href="#NOI">Jump to Non-Observable Issues</a>



### True Positives### {#TP}

| **Report Type** | **Web Page** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| CloudConvert | [1](../CloudConvert-failure-1.html#About-drlf) | 980px-980px | TP | Header and main content panel clearly overlapping, obscuring the banner [Screenshot and Detailed Information](../CloudConvert-failure-1.html) |
| Element Collision| MidwayMeetup | [2](../MidwayMeetup-failure-2.html#About-drlf) | 768px-1132px | TP | Form is clearly overlapping with the main panel, and button is unclickable [Screenshot and Detailed Information](../MidwayMeetup-failure-2.html) |
| Element Collision| PepFeed | [3](../PepFeed-failure-4.html#About-drlf) | 415px-546px | TP | Panels 1 and 2 clearly overlapping [Screenshot and Detailed Information](../PepFeed-failure-4.html) |
| Element Collision| PepFeed | [4](../PepFeed-failure-8.html#About-drlf) | 547px-700px | TP | Panels 1 and 3 clearly overlapping [Screenshot and Detailed Information](../PepFeed-failure-8.html) |
| Element Collision| PepFeed | [5](../PepFeed-failure-9.html#About-drlf) | 769px-933px | TP | Panels 1 and 3 clearly overlapping [Screenshot and Detailed Information](../PepFeed-failure-9.html) |
| Element Collision| PepFeed | [6](../PepFeed-failure-10.html#About-drlf) | 415px-415px | TP | Panels 2 and 3 clearly overlapping [Screenshot and Detailed Information](../PepFeed-failure-10.html) |
| Element Collision| StumbleUpon | [7](../StumbleUpon-failure-1.html#About-drlf) | 320px-439px | TP | Element collision clearly causing undesirable layout [Screenshot and Detailed Information](../StumbleUpon-failure-1.html) |
| Element Collision| WillMyPhoneWork | [8](../WillMyPhoneWork-failure-1.html#About-drlf) | 990px-991px | TP | Header and main content clearly overlapping [Screenshot and Detailed Information](../WillMyPhoneWork-failure-1.html) |
| Element Protrusion| BugMeNot | [9](../BugMeNot-failure-4.html#About-drlf) | 403px-678px | TP | Form is clearly protruding out of the page's header. [Screenshot and Detailed Information](../BugMeNot-failure-4.html) |
| Element Protrusion| Consumer-Reports | [10](../Consumer-Reports-failure-14.html#About-drlf) | 392px-767px | TP | Text has clearly protruding outside its container [Screenshot and Detailed Information](../Consumer-Reports-failure-14.html) |
| Element Protrusion| Pdf-Escape | [11](../Pdf-Escape-failure-8.html#About-drlf) | 801px-805px | TP | Navigation links have clearly protruded outside the navbar and become invisible and unclickable [Screenshot and Detailed Information](../Pdf-Escape-failure-8.html) |
| Viewport Protrusion| 3-Minute-Journal | [12](../3-Minute-Journal-failure-1.html#About-drlf) | 320px-371px | TP | 'Feb' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-1.html) |
| Viewport Protrusion| 3-Minute-Journal | [12](../3-Minute-Journal-failure-2.html#About-drlf) | 320px-583px | TP | 'July' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-2.html) |
| Viewport Protrusion| 3-Minute-Journal | [13](../3-Minute-Journal-failure-3.html#About-drlf) | 992px-1136px | TP | 'July' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-3.html) |
| Viewport Protrusion| 3-Minute-Journal | [12](../3-Minute-Journal-failure-4.html#About-drlf) | 320px-413px | TP | 'Mar' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-4.html) |
| Viewport Protrusion| 3-Minute-Journal | [12](../3-Minute-Journal-failure-5.html#About-drlf) | 320px-437px | TP | 'Apr' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-5.html) |
| Viewport Protrusion| 3-Minute-Journal | [12](../3-Minute-Journal-failure-6.html#About-drlf) | 320px-542px | TP | 'Jun' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-6.html) |
| Viewport Protrusion| 3-Minute-Journal | [13](../3-Minute-Journal-failure-7.html#About-drlf) | 992px-1055px | TP | 'Jun' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-7.html) |
| Viewport Protrusion| 3-Minute-Journal | [12](../3-Minute-Journal-failure-8.html#About-drlf) | 320px-499px | TP | 'May' label outside the viewport [Screenshot and Detailed Information](../3-Minute-Journal-failure-8.html) |
| Viewport Protrusion| BugMeNot | [14](../BugMeNot-failure-1.html#About-drlf) | 320px-353px | TP | Part of input box obscured by viewport protrusion, so a TP [Screenshot and Detailed Information](../BugMeNot-failure-1.html) |
| Viewport Protrusion| BugMeNot | [15](../BugMeNot-failure-2.html#About-drlf) | 320px-340px | TP | Part of input box obscured by viewport protrusion, so a TP [Screenshot and Detailed Information](../BugMeNot-failure-2.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-4.html#About-drlf) | 320px-365px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-4.html) |
| Viewport Protrusion| Consumer-Reports | [17](../Consumer-Reports-failure-5.html#About-drlf) | 1025px-1110px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-5.html) |
| Viewport Protrusion| Consumer-Reports | [18](../Consumer-Reports-failure-6.html#About-drlf) | 768px-1039px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-6.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-7.html#About-drlf) | 320px-377px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-7.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-8.html#About-drlf) | 320px-375px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-8.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-9.html#About-drlf) | 320px-377px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-9.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-10.html#About-drlf) | 320px-377px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-10.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-11.html#About-drlf) | 320px-375px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-11.html) |
| Viewport Protrusion| Consumer-Reports | [16](../Consumer-Reports-failure-12.html#About-drlf) | 320px-375px | TP | Element clearly protruding outside of the viewport [Screenshot and Detailed Information](../Consumer-Reports-failure-12.html) |
| Viewport Protrusion| Duolingo | [19](../Duolingo-failure-1.html#About-drlf) | 981px-1099px | TP | Carousel is clearly protruding outside the viewport [Screenshot and Detailed Information](../Duolingo-failure-1.html) |
| Viewport Protrusion| Duolingo | [19](../Duolingo-failure-3.html#About-drlf) | 981px-1099px | TP | Carousel is clearly protruding outside the viewport [Screenshot and Detailed Information](../Duolingo-failure-3.html) |
| Viewport Protrusion| HotelWifiTest | [20](../HotelWifiTest-failure-1.html#About-drlf) | 415px-767px | TP | Main container clearly protruding from the viewport, obscuring lots of content [Screenshot and Detailed Information](../HotelWifiTest-failure-1.html) |
| Viewport Protrusion| Pdf-Escape | [21](../Pdf-Escape-failure-4.html#About-drlf) | 768px-850px | TP | Part of image obscured by protrusion outside viewport [Screenshot and Detailed Information](../Pdf-Escape-failure-4.html) |
| Viewport Protrusion| PepFeed | [22](../PepFeed-failure-1.html#About-drlf) | 415px-768px | TP | Amazon logo obscured by viewport at narrower width than screenshot. [Screenshot and Detailed Information](../PepFeed-failure-1.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-1.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-1.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-2.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-2.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-3.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-3.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-4.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-4.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-5.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-5.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-6.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-6.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-7.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-7.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-8.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-8.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-9.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-9.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-10.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-10.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-11.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-11.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-12.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-12.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-13.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-13.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-14.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-14.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-15.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-15.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-16.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-16.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-17.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-17.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-18.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-18.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-19.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-19.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-20.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-20.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-21.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-21.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-22.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-22.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-23.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-23.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-24.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-24.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-25.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-25.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-26.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-26.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-27.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-27.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-28.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-28.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-29.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-29.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-30.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-30.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-31.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-31.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-32.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-32.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-33.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-33.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-34.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-34.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-35.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-35.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-36.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-36.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-37.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-37.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-38.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-38.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-39.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-39.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-40.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-40.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-41.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-41.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-42.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-42.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-43.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-43.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-44.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-44.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-45.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-45.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-46.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-46.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-47.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-47.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-48.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-48.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-49.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-49.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-50.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-50.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-51.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-51.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-52.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-52.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-54.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-54.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-55.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-55.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-56.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-56.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-57.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-57.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-58.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-58.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-59.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-59.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-61.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-61.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-62.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-62.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-63.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-63.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-64.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-64.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-65.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-65.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-66.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-66.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-67.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-67.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-68.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-68.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-70.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-70.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-71.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-71.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-72.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-72.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-73.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-73.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-74.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-74.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-75.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-75.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-76.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-76.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-77.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-77.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-78.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-78.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-79.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-79.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-80.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-80.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-81.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-81.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-82.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-82.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-83.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-83.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-84.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-84.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-85.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-85.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-86.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-86.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-87.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-87.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-88.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-88.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-89.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-89.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-90.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-90.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-91.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-91.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-92.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-92.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-93.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-93.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-94.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-94.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-95.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-95.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-96.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-96.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-97.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-97.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-98.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-98.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-99.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-99.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-100.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-100.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-101.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-101.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-102.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-102.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-103.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-103.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-104.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-104.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-105.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-105.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-106.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-106.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-107.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-107.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-108.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-108.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-109.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-109.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-110.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-110.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-111.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-111.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-112.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-112.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-113.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-113.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-114.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-114.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-115.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-115.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-116.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-116.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-117.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-117.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-118.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-118.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-119.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-119.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-120.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-120.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-121.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-121.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-123.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-123.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-124.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-124.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-125.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-125.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-126.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-126.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-127.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-127.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-128.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-128.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-129.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-129.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-130.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-130.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-131.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-131.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-132.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-132.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-133.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-133.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-134.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-134.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-135.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-135.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-136.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-136.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-137.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-137.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-138.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-138.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-139.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-139.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-140.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-140.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-141.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-141.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-142.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-142.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-143.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-143.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-145.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-145.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-146.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-146.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-147.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-147.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-148.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-148.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-149.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-149.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-150.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-150.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-151.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-151.html) |
| Small-Range| AccountKiller | [23](../AccountKiller-failure-152.html#About-drlf) | 476px-480px | TP | Layout only true from 476-480px, so a TP [Screenshot and Detailed Information](../AccountKiller-failure-152.html) |
| Small-Range| CloudConvert | [1](../CloudConvert-failure-2.html#About-drlf) | 980px-980px | TP | Layout only true at 980px, so clearly a TP. [Screenshot and Detailed Information](../CloudConvert-failure-2.html) |
| Small-Range| PepFeed | [6](../PepFeed-failure-24.html#About-drlf) | 415px-415px | TP | Layout only true for 415px, so a TP. [Screenshot and Detailed Information](../PepFeed-failure-24.html) |
| Small-Range| PepFeed | [6](../PepFeed-failure-26.html#About-drlf) | 415px-415px | TP | Layout only true for 415px, so a TP. [Screenshot and Detailed Information](../PepFeed-failure-26.html) |
| Small-Range| WillMyPhoneWork | [8](../WillMyPhoneWork-failure-3.html#About-drlf) | 990px-991px | TP | Elements are only overlapping for a couple of widths, so a TP [Screenshot and Detailed Information](../WillMyPhoneWork-failure-3.html) |
| Small-Range| WillMyPhoneWork | [8](../WillMyPhoneWork-failure-4.html#About-drlf) | 990px-991px | TP | Alignment only true for a couple of widths, so a TP [Screenshot and Detailed Information](../WillMyPhoneWork-failure-4.html) |
| Wrapping| AccountKiller | [24](../AccountKiller-failure-153.html#About-drlf) | 394px-459px | TP | Tweet icon clearly wrapped onto a new row [Screenshot and Detailed Information](../AccountKiller-failure-153.html) |
| Wrapping| AccountKiller | [25](../AccountKiller-failure-154.html#About-drlf) | 808px-959px | TP | 'The Atlantic' clearly wrapped onto a new row [Screenshot and Detailed Information](../AccountKiller-failure-154.html) |
| Wrapping| AirBnb | [26](../AirBnb-failure-12.html#About-drlf) | 321px-335px | TP | 'Terms and Privacy' clearly wrapped onto new row [Screenshot and Detailed Information](../AirBnb-failure-12.html) |
| Wrapping| AirBnb | [27](../AirBnb-failure-13.html#About-drlf) | 326px-356px | TP | Instagram logo clearly wrapped onto new row [Screenshot and Detailed Information](../AirBnb-failure-13.html) |
| Wrapping| BugMeNot | [28](../BugMeNot-failure-7.html#About-drlf) | 456px-514px | TP | Search button has wrapped onto a new line. [Screenshot and Detailed Information](../BugMeNot-failure-7.html) |
| Wrapping| Covered-Calendar | [29](../Covered-Calendar-failure-4.html#About-drlf) | 320px-385px | TP | 'Privacy Policy' cleared wraps onto a new line [Screenshot and Detailed Information](../Covered-Calendar-failure-4.html) |
| Wrapping| Covered-Calendar | [30](../Covered-Calendar-failure-5.html#About-drlf) | 768px-979px | TP | Header navigation link clearly wraps onto a new line [Screenshot and Detailed Information](../Covered-Calendar-failure-5.html) |
| Wrapping| Ninite | [31](../Ninite-failure-2.html#About-drlf) | 347px-395px | TP | 'terms' nav link clearly wrapped onto new line [Screenshot and Detailed Information](../Ninite-failure-2.html) |
| Wrapping| PepFeed | [32](../PepFeed-failure-28.html#About-drlf) | 320px-386px | TP | 'The Verge' has clearly wrapped onto a new line [Screenshot and Detailed Information](../PepFeed-failure-28.html) |
| Wrapping| UserSearch | [33](../UserSearch-failure-2.html#About-drlf) | 625px-794px | TP | Final navigation link clearly wrapped onto a new line [Screenshot and Detailed Information](../UserSearch-failure-2.html) |

### False Positives### {#FP}

| **Report Type** | **Web Page** | **Viewport Range** | **Classification** | **Reason** |
| Small-Range| 3-Minute-Journal | 764px-767px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../3-Minute-Journal-failure-12.html) |
| Small-Range| AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../AccountKiller-failure-53.html) |
| Small-Range| AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../AccountKiller-failure-60.html) |
| Small-Range| AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../AccountKiller-failure-69.html) |
| Small-Range| AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../AccountKiller-failure-122.html) |
| Small-Range| AccountKiller | 800px-803px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../AccountKiller-failure-144.html) |
| Small-Range| AirBnb | 1199px-1199px | FP | Element is not visibly protruding [Screenshot and Detailed Information](../AirBnb-failure-10.html) |
| Small-Range| AirBnb | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../AirBnb-failure-11.html) |
| Small-Range| Consumer-Reports | 768px-770px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../Consumer-Reports-failure-24.html) |
| Small-Range| Duolingo | 378px-380px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../Duolingo-failure-6.html) |
| Small-Range| Honey | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../Honey-failure-11.html) |
| Small-Range| Honey | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../Honey-failure-12.html) |
| Small-Range| Honey | 1200px-1200px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../Honey-failure-13.html) |
| Small-Range| HotelWifiTest | 992px-992px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../HotelWifiTest-failure-2.html) |
| Small-Range| HotelWifiTest | 769px-769px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../HotelWifiTest-failure-3.html) |
| Small-Range| Mailinator | 499px-502px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../Mailinator-failure-2.html) |
| Small-Range| Mailinator | 499px-502px | FP | No significant layout change, just coincidental labelling [Screenshot and Detailed Information](../Mailinator-failure-3.html) |
| Small-Range| PepFeed | 480px-480px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-12.html) |
| Small-Range| PepFeed | 732px-736px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-13.html) |
| Small-Range| PepFeed | 598px-600px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-14.html) |
| Small-Range| PepFeed | 748px-750px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-15.html) |
| Small-Range| PepFeed | 1024px-1024px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-16.html) |
| Small-Range| PepFeed | 992px-993px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-17.html) |
| Small-Range| PepFeed | 965px-965px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-18.html) |
| Small-Range| PepFeed | 480px-480px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-19.html) |
| Small-Range| PepFeed | 748px-750px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-20.html) |
| Small-Range| PepFeed | 598px-600px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-21.html) |
| Small-Range| PepFeed | 732px-736px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-22.html) |
| Small-Range| PepFeed | 769px-773px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-23.html) |
| Small-Range| PepFeed | 1200px-1202px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-25.html) |
| Small-Range| PepFeed | 992px-993px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../PepFeed-failure-27.html) |
| Small-Range| Pocket | 768px-770px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../Pocket-failure-6.html) |
| Small-Range| Pocket | 768px-768px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../Pocket-failure-7.html) |
| Small-Range| Pocket | 768px-770px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../Pocket-failure-8.html) |
| Small-Range| RunPee | 479px-479px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../RunPee-failure-1.html) |
| Small-Range| RunPee | 480px-483px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../RunPee-failure-2.html) |
| Small-Range| RunPee | 480px-480px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../RunPee-failure-3.html) |
| Small-Range| RunPee | 481px-481px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../RunPee-failure-4.html) |
| Small-Range| RunPee | 768px-772px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../RunPee-failure-5.html) |
| Small-Range| TopDocumentary | 689px-691px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../TopDocumentary-failure-12.html) |
| Small-Range| TopDocumentary | 593px-596px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../TopDocumentary-failure-13.html) |
| Small-Range| ZeroDollarMovies | 481px-483px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../ZeroDollarMovies-failure-1.html) |
| Small-Range| ZeroDollarMovies | 481px-481px | FP | No significant layout change, just coincidental attribute labelling [Screenshot and Detailed Information](../ZeroDollarMovies-failure-2.html) |
| Wrapping| Duolingo | 378px-399px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../Duolingo-failure-7.html) |
| Wrapping| Duolingo | 830px-881px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../Duolingo-failure-8.html) |
| Wrapping| Ninite | 410px-614px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../Ninite-failure-1.html) |
| Wrapping| RunPee | 480px-681px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../RunPee-failure-6.html) |
| Wrapping| StumbleUpon | 661px-840px | FP | Intentional layout change causes element to appear on separate row [Screenshot and Detailed Information](../StumbleUpon-failure-2.html) |

### Non-Observable Issues### {#NOI}

| **Report Type** | **Web Page** | **Viewport Range** | **Classification** | **Reason** |
| Element Collision| 3-Minute-Journal | 320px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../3-Minute-Journal-failure-9.html) |
| Element Collision| AirBnb | 744px-1127px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../AirBnb-failure-5.html) |
| Element Collision| Consumer-Reports | 336px-767px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../Consumer-Reports-failure-15.html) |
| Element Collision| Consumer-Reports | 320px-384px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Consumer-Reports-failure-16.html) |
| Element Collision| Consumer-Reports | 648px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Consumer-Reports-failure-18.html) |
| Element Collision| Consumer-Reports | 320px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Consumer-Reports-failure-20.html) |
| Element Collision| Consumer-Reports | 691px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Consumer-Reports-failure-21.html) |
| Element Collision| Consumer-Reports | 329px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Consumer-Reports-failure-22.html) |
| Element Collision| Consumer-Reports | 320px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Consumer-Reports-failure-23.html) |
| Element Collision| Duolingo | 320px-980px | NOI | No overlap of visual content, just DOM coordinates [Screenshot and Detailed Information](../Duolingo-failure-5.html) |
| Element Collision| Mailinator | 992px-1199px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Mailinator-failure-1.html) |
| Element Collision| PepFeed | 415px-479px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../PepFeed-failure-5.html) |
| Element Collision| PepFeed | 320px-479px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../PepFeed-failure-6.html) |
| Element Collision| PepFeed | 934px-965px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../PepFeed-failure-11.html) |
| Element Collision| Pocket | 487px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Pocket-failure-1.html) |
| Element Collision| Pocket | 487px-767px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../Pocket-failure-2.html) |
| Element Collision| TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-1.html) |
| Element Collision| TopDocumentary | 765px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-2.html) |
| Element Collision| TopDocumentary | 682px-688px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-5.html) |
| Element Collision| TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-6.html) |
| Element Collision| TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-8.html) |
| Element Collision| TopDocumentary | 785px-944px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-9.html) |
| Element Collision| TopDocumentary | 681px-688px | NOI | No overlap of content, just DOM coordinates [Screenshot and Detailed Information](../TopDocumentary-failure-10.html) |
| Element Collision| UserSearch | 802px-897px | NOI | No visible content overlap, just DOM coordinates [Screenshot and Detailed Information](../UserSearch-failure-1.html) |
| Element Protrusion| 3-Minute-Journal | 438px-449px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../3-Minute-Journal-failure-10.html) |
| Element Protrusion| 3-Minute-Journal | 992px-1199px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../3-Minute-Journal-failure-11.html) |
| Element Protrusion| AirBnb | 320px-743px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../AirBnb-failure-6.html) |
| Element Protrusion| AirBnb | 320px-743px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../AirBnb-failure-7.html) |
| Element Protrusion| AirBnb | 744px-768px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../AirBnb-failure-8.html) |
| Element Protrusion| AirBnb | 320px-743px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../AirBnb-failure-9.html) |
| Element Protrusion| BugMeNot | 335px-529px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../BugMeNot-failure-3.html) |
| Element Protrusion| BugMeNot | 320px-420px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../BugMeNot-failure-5.html) |
| Element Protrusion| BugMeNot | 320px-334px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../BugMeNot-failure-6.html) |
| Element Protrusion| Consumer-Reports | 771px-1180px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../Consumer-Reports-failure-13.html) |
| Element Protrusion| Consumer-Reports | 771px-1180px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../Consumer-Reports-failure-17.html) |
| Element Protrusion| Consumer-Reports | 320px-767px | NOI | Element is not visible protruding [Screenshot and Detailed Information](../Consumer-Reports-failure-19.html) |
| Element Protrusion| Honey | 1200px-1200px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-3.html) |
| Element Protrusion| Honey | 1001px-1199px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-4.html) |
| Element Protrusion| Honey | 320px-1199px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-5.html) |
| Element Protrusion| Honey | 1200px-1200px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-6.html) |
| Element Protrusion| Honey | 320px-325px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-7.html) |
| Element Protrusion| Honey | 566px-767px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-8.html) |
| Element Protrusion| Honey | 682px-767px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-9.html) |
| Element Protrusion| Honey | 320px-325px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Honey-failure-10.html) |
| Element Protrusion| MidwayMeetup | 768px-1024px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../MidwayMeetup-failure-3.html) |
| Element Protrusion| Pdf-Escape | 843px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pdf-Escape-failure-5.html) |
| Element Protrusion| Pdf-Escape | 768px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pdf-Escape-failure-6.html) |
| Element Protrusion| Pdf-Escape | 768px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pdf-Escape-failure-7.html) |
| Element Protrusion| Pdf-Escape | 320px-479px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pdf-Escape-failure-9.html) |
| Element Protrusion| Pdf-Escape | 768px-959px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pdf-Escape-failure-10.html) |
| Element Protrusion| PepFeed | 768px-991px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../PepFeed-failure-3.html) |
| Element Protrusion| PepFeed | 768px-991px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../PepFeed-failure-7.html) |
| Element Protrusion| Pocket | 768px-900px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pocket-failure-3.html) |
| Element Protrusion| Pocket | 877px-885px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pocket-failure-4.html) |
| Element Protrusion| Pocket | 877px-885px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../Pocket-failure-5.html) |
| Element Protrusion| TopDocumentary | 509px-512px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../TopDocumentary-failure-3.html) |
| Element Protrusion| TopDocumentary | 566px-944px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../TopDocumentary-failure-4.html) |
| Element Protrusion| TopDocumentary | 549px-944px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../TopDocumentary-failure-7.html) |
| Element Protrusion| TopDocumentary | 558px-944px | NOI | Element is not visibly protruding [Screenshot and Detailed Information](../TopDocumentary-failure-11.html) |
| Element Protrusion| WillMyPhoneWork | 992px-1199px | NOI | Element is not visibly protruding from its parent [Screenshot and Detailed Information](../WillMyPhoneWork-failure-2.html) |
| Viewport Protrusion| AirBnb | 320px-743px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../AirBnb-failure-1.html) |
| Viewport Protrusion| AirBnb | 320px-743px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../AirBnb-failure-2.html) |
| Viewport Protrusion| AirBnb | 320px-710px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../AirBnb-failure-3.html) |
| Viewport Protrusion| AirBnb | 744px-1073px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../AirBnb-failure-4.html) |
| Viewport Protrusion| Consumer-Reports | 768px-782px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../Consumer-Reports-failure-1.html) |
| Viewport Protrusion| Consumer-Reports | 1200px-1400px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../Consumer-Reports-failure-2.html) |
| Viewport Protrusion| Consumer-Reports | 768px-782px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../Consumer-Reports-failure-3.html) |
| Viewport Protrusion| Covered-Calendar | 1200px-1240px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../Covered-Calendar-failure-1.html) |
| Viewport Protrusion| Covered-Calendar | 1200px-1240px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../Covered-Calendar-failure-2.html) |
| Viewport Protrusion| Covered-Calendar | 1200px-1240px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../Covered-Calendar-failure-3.html) |
| Viewport Protrusion| Days-Old | 320px-340px | NOI | No visible protrusion outside the viewport [Screenshot and Detailed Information](../Days-Old-failure-1.html) |
| Viewport Protrusion| Dictation | 320px-480px | NOI | No visible protrusion outside the viewport [Screenshot and Detailed Information](../Dictation-failure-1.html) |
| Viewport Protrusion| Duolingo | 981px-1276px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Duolingo-failure-2.html) |
| Viewport Protrusion| Duolingo | 981px-1267px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Duolingo-failure-4.html) |
| Viewport Protrusion| Honey | 768px-789px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Honey-failure-1.html) |
| Viewport Protrusion| Honey | 992px-1009px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Honey-failure-2.html) |
| Viewport Protrusion| MidwayMeetup | 320px-535px | NOI | No visible protrusion of element outside the viewport [Screenshot and Detailed Information](../MidwayMeetup-failure-1.html) |
| Viewport Protrusion| Pdf-Escape | 320px-800px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Pdf-Escape-failure-1.html) |
| Viewport Protrusion| Pdf-Escape | 768px-780px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Pdf-Escape-failure-2.html) |
| Viewport Protrusion| Pdf-Escape | 960px-972px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../Pdf-Escape-failure-3.html) |
| Viewport Protrusion| PepFeed | 1025px-1080px | NOI | No content obscured by viewport protrusion [Screenshot and Detailed Information](../PepFeed-failure-2.html) |
| Viewport Protrusion| WhatShouldIReadNext | 601px-611px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../WhatShouldIReadNext-failure-1.html) |
| Viewport Protrusion| WhatShouldIReadNext | 601px-611px | NOI | No content obscured by viewport protrusion, so just an NOI [Screenshot and Detailed Information](../WhatShouldIReadNext-failure-2.html) |
