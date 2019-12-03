---
edit-last: 4
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
pubDate: Fri, 04 Jul 2014 16:14:39 +0000
dc-creator: hchang@adobe.com
guid: https://education.tubemogul.com/userguide/?page_id=1545
isPermaLink: false
description: 
postId: 1545
postDate: 2014-07-04 08:14:39
postDateGmt: 2014-07-04 16:14:39
commentStatus: open
pingStatus: closed
postName: conversions
status: publish
postParent: 1428
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Conversions {#conversions}

Advertising Cloud DSP tracks and reports conversion metrics (that is, impressions conversions, view conversions, and click conversions) for every conversion pixel built within the platform. Conversion reporting is available on the dashboard as well as through [Email Reports](../../../dsp/measurement/campaign-reporting/email-reports.md).

A conversion pixel is a piece of code that's put on a website (often an advertiser's landing page, but possibly a publisher) to track a post-ad experience action, such as registering as a Facebook fan, filling out a form, or buying a product. The conversion action is completely up to the advertiser and how they implement the pixel on their site.

For display ads, conversion pixels typically track:

* Click-through - User clicked on the ad to get to the conversion site
* View-through - User viewed an ad and went to the conversion site sometime later

Video ads can track the following metrics:

* Click conversion - User clicked on the ad and either directly landed on the conversion page, or converted sometime later
* View conversion - User viewed the video and went to the conversion page sometime later
* Impression conversion - User was exposed to an in-banner impression and went to the conversion page sometime later

Note that a view conversion in Advertising Cloud DSP is not quite the same thing as a "view-through" conversion in the display world.

Conversion pixels also support the notion of a "lookback window".  This defines the trailing time period for which the original activity with the ad will be considered eligible for conversion.  By default, all conversion types have a lookback window of 30 days.  That means that if the ad was seen 40 days ago, before the conversion page was hit, it would not be considered a valid conversion and wouldn't be counted.

The best practice is to [create a conversion pixel](conversions/conversion-pixel-setup.md) at least a week before you launch a campaign to ensure proper implementation and pixel firing. Once a conversion pixel is implemented, enable it in a placement.
