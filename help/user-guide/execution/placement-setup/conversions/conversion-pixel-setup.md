---
edit-last: 4
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Wed, 16 Jul 2014 07:19:08 +0000
dc-creator: hthomas@adobe.com
guid: https://education.tubemogul.com/?page_id=2225
isPermaLink: false
description: 
postId: 2225
postDate: 2014-07-15 23:19:08
postDateGmt: 2014-07-16 07:19:08
commentStatus: open
pingStatus: open
postName: conversion-pixel-setup
status: publish
postParent: 1545
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Conversion Pixel Setup {#conversion-pixel-setup}
1. Create a conversion pixel:
  1. In the main menu, click **DSP > Tools > Conversions**.
  1. Click **New Conversion**.
  1. Select the advertiser.
  1. Specify the pixel settings, including:
    * Campaigns: The applicable campaigns. The pixel is enabled by default for any new placements created for the selected campaigns, but not to existing placements.
    * Name: The name of the pixel.
    * Notes: (Optional) Any notes for your information.
    * Conversion Category: The type of conversion. <!-- Do these change the format of the pixel code? Add info. about each, or at least an exanple of how each will look. -->
    * The lookback windows for different viewer actions:
      * <*N*> days after an impression: The number of days after an ad impression occurs in which the impression can be attributed to a conversion. 
      * <*N*> days after a view: The number of days after the first view occurs in which the view can be attributed to a conversion. 
      * <*N*> days after a click: The number of days after the first click occurs in which the click can be attributed to a conversion.
  1.  Click **Add**.
1. Copy the HTML tag and insert it in the website pages on which the conversion takes place, and insert the Flash tag within any Flash applications in which the conversion takes place.

  [ ![image2013-3-25 13-34-24](assets/image2013-3-25-13-34-24.jpeg)](assets/image2013-3-25-13-34-24.jpeg)

1. Verify the conversion is firing with a web developer tool, such as Charles, Firebug, or Fiddler.
1. (If the campaigns for which the pixel applies already include placements) Manually edit the applicable placement settings to add the pixel.


## Attribution

Attribution of the conversion refers to the decision of which ad to associate the conversion to, from a potential set of ads the user was exposed to. The industry norm is to use a "last-touch" attribution. However, there are some precedence rules that come into play as well.
Our current model uses this approach:

1. Click-throughs on any ads enabled for this conversion pixel are considered first. The most recently clicked ad within the lookback window receives the conversion.
1. Video views on any ads enabled for this conversion pixel  are considered next. The most recently viewed ad within the lookback window receives the conversion.
1. In-banner impressions on any ads enabled for this conversion pixel  are considered last. The most recently exposed impression within the lookback window receives the conversion.

Note: Only one conversion every 24 hours is permitted per user, per conversion-pixel.

## Possible Stats Discrepancies

* Other ad servers may not limit against the user + conversion pixel. So for sites that have multiple conversion pixels, we will attribute a conversion to the user landing on each one. Other ad servers may limit this more strictly, ie. only allow one conversion per placement or creative.
* Browser that don't allow 3rd-party cookies will not properly count conversions.
* Often people may compare click-throughs to conversions. However, these can be quite mismatched, for reasons such as:

  * If the click-through doesn't go through directly to the page the conversion pixel is on, ie. it requires more user activity (sign-up, check-out, etc.) before the pixel fires.
  * A person can only convert on the same ad once every 24 hours. Often we see multiple clicks by the same user, so these are filtered out.
  * Popup blockers may prevent the actual window from opening, even though we've counted the click-through.
  * People may leave the landing page before the conversion pixel fires.
