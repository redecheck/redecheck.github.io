---
layout: post
title: "AccountKiller"
elements: 343
decs: 559
fullurl: www.accountkiller.com/en
---

## Distinct RLFs

| RLF No. | Type | Description | Screenshot (Bad) | Screenshot (OK) |
| 3 | Small-Range | Some tiles shift location for 476px-480px. While not strictly 'bad' in terms of aesthetics, notifying a developer of this layout shift would likely still be useful. Given how few viewport widths it manifests at, it would likely be very difficult and time-consuming for developer to manually detect it. | [478px]({{ site.baseurl }}/assets/good-bad/rlf3/478.png) |  [475px]({{ site.baseurl }}/assets/good-bad/rlf3/475.png)  [481px]({{ site.baseurl }}/assets/good-bad/rlf3/481.png)|
| 4 | Wrapping | 'The Atlantic' wraps onto a new line. No impact on functionality, but aesthetically, two rows of three icons might look much more professional. Eventually the elements all wrap so they are in 2 rows of 3 and then 3 rows of 2, but a developer should probably use media queries to implement this rather than relying on the incongruously wrapping of the elements. | [Bad]({{ site.baseurl }}/assets/good-bad/rlf4/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf4/ok.png) |
| 5 | Wrapping | 'Tweet' icon wraps onto a new line. No impact on functionality again, but does detrimentally impact the looks given all the other icons are shown in a single row. As the viewport continues to narrow, more elements wrap onto the second line which improves the layout a little, but a media query to switch the layout prior to the wrapping behaviour would likely be considered better RWD. | [Bad]({{ site.baseurl }}/assets/good-bad/rlf5/bad.png) | [OK]({{ site.baseurl }}/assets/good-bad/rlf5/ok.png) |

All three of these RLFs are still currently manifesting on the live version of the site, which is viewable [here](https://www.accountkiller.com/en/#).

## Full Results

| Failure No. | Category | Screenshot | Classification | Reason | Distinct RLF |
| 1| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault1/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 2| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault2/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 3| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault3/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 4| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault4/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 5| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault5/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 6| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault6/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 7| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault7/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 8| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault8/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 9| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault9/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 10| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault10/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 11| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault11/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 12| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault12/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 13| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault13/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 14| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault14/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 15| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault15/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 16| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault16/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 17| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault17/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 18| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault18/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 19| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault19/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 20| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault20/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 21| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault21/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 22| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault22/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 23| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault23/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 24| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault24/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 25| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault25/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 26| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault26/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 27| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault27/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 28| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault28/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 29| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault29/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 30| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault30/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 31| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault31/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 32| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault32/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 33| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault33/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 34| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault34/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 35| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault35/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 36| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault36/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 37| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault37/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 38| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault38/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 39| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault39/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 40| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault40/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 41| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault41/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 42| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault42/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 43| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault43/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 44| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault44/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 45| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault45/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 46| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault46/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 47| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault47/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 48| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault48/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 49| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault49/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 50| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault50/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 51| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault51/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 52| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault52/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 53| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault53/smallrangeWidth801.png) | FP | No significant layout change, just coincidental attribute labelling | |
| 54| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault54/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 55| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault55/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 56| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault56/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 57| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault57/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 58| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault58/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 59| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault59/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 60| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault60/smallrangeWidth801.png) | FP | No significant layout change, just coincidental attribute labelling | |
| 61| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault61/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 62| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault62/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 63| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault63/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 64| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault64/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 65| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault65/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 66| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault66/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 67| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault67/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 68| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault68/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 69| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault69/smallrangeWidth801.png) | FP | No significant layout change, just coincidental attribute labelling | |
| 70| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault70/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 71| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault71/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 72| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault72/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 73| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault73/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 74| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault74/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 75| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault75/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 76| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault76/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 77| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault77/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 78| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault78/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 79| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault79/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 80| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault80/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 81| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault81/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 82| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault82/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 83| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault83/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 84| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault84/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 85| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault85/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 86| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault86/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 87| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault87/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 88| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault88/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 89| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault89/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 90| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault90/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 91| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault91/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 92| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault92/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 93| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault93/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 94| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault94/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 95| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault95/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 96| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault96/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 97| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault97/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 98| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault98/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 99| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault99/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 100| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault100/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 101| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault101/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 102| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault102/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 103| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault103/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 104| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault104/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 105| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault105/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 106| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault106/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 107| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault107/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 108| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault108/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 109| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault109/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 110| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault110/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 111| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault111/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 112| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault112/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 113| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault113/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 114| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault114/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 115| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault115/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 116| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault116/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 117| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault117/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 118| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault118/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 119| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault119/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 120| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault120/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 121| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault121/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 122| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault122/smallrangeWidth801.png) | FP | No significant layout change, just coincidental attribute labelling | |
| 123| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault123/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 124| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault124/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 125| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault125/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 126| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault126/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 127| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault127/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 128| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault128/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 129| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault129/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 130| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault130/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 131| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault131/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 132| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault132/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 133| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault133/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 134| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault134/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 135| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault135/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 136| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault136/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 137| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault137/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 138| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault138/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 139| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault139/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 140| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault140/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 141| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault141/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 142| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault142/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 143| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault143/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 144| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault144/smallrangeWidth801.png) | FP | No significant layout change, just coincidental attribute labelling | |
| 145| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault145/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 146| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault146/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 147| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault147/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 148| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault148/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 149| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault149/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 150| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault150/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 151| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault151/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 152| Small-Range | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault152/smallrangeWidth478.png) | TP | Layout only true from 476-480px, so a TP | 3 |
| 153| Wrapping | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault153/wrappingWidth426.png) | TP | Tweet icon clearly wrapped onto a new row | 4 |
| 154| Wrapping | [Click]({{ site.baseurl }}/assets/images/AccountKiller/fault154/wrappingWidth883.png) | TP | 'The Atlantic' clearly wrapped onto a new row | 5|
