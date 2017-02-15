---
layout: post
title: "AccountKiller Fault 84"
---
| **Report Type** | **Distinct RLF No.** | **Viewport Range** | **Classification** | **Reason** |
| Small-Range| 23 | 476px-480px | TP | Layout only true from 476-480px, so a TP | 

![Screenshot of the fault]({{ site.baseurl }}/assets/images/AccountKiller/fault84/smallrangeWidth478.png){: .center-image }

## About Distinct RLF 23

Some tiles shift location for 476px-480px. While not strictly 'bad' in terms of aesthetics, notifying a developer of this layout shift would likely still be useful. Given how few viewport widths the failure manifests at, detecting it with a manual approach would likely be difficult. The failure is currently still manifesting in the live site, available [here](http://www.accountkiller.com/en/).

At 475px, the tiles are laid out in two columns:

![475px]({{ site.baseurl }}/assets/good-bad/rlf3/475.png){: .center-image}

But from 476-480px, they shift into a three column layout:

![478px]({{ site.baseurl }}/assets/good-bad/rlf3/478.png){: .center-image}

Then, at 481px, it reverts to a two column layout:

![481px]({{ site.baseurl }}/assets/good-bad/rlf3/481.png){: .center-image}
