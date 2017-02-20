---
layout: post
title: "AccountKiller Failure 133"
---
| **Report Type** | **Distinct RLF** | **Viewport Range** | **Classification** | **Reason** |
| Small-Range| 23 | 476px-480px | TP | Layout only true from 476-480px, so a TP | 

![Screenshot of the fault](../../../assets/images/AccountKiller/fault133/smallrangeWidth478.png){: .center-image }

## About Distinct RLF 23

Some tiles shift location for 476px-480px. While not strictly 'bad' in terms of aesthetics, notifying a developer of this layout shift would likely still be useful. Given how few viewport widths the failure manifests at, detecting it with a manual approach would likely be difficult. The failure is currently still manifesting in the live site, available [here](http://www.accountkiller.com/en/).

At 475px, the tiles are laid out in two columns:

![475px](../../../assets/good-bad/rlf23/475.png){: .center-image}

But from 476-480px, they shift into a three column layout:

![478px](../../../assets/good-bad/rlf23/478.png){: .center-image}

Then, at 481px, it reverts to a two column layout:

![481px](../../../assets/good-bad/rlf23/481.png){: .center-image}
