---
edit-last: 3
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
pubDate: Wed, 16 Jul 2014 07:19:42 +0000
dc-creator: hthomas@adobe.com
guid: http://education.tubemogul.com/?page_id=2217
isPermaLink: false
description: 
postId: 2217
postDate: 2014-07-15 23:19:42
postDateGmt: 2014-07-16 07:19:42
commentStatus: open
pingStatus: open
postName: conversions-2
status: publish
postParent: 2241
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Conversions {#conversions}

TubeMogul enables you to easily track and report on every conversion pixel built within the platform. Reporting is accessible on the dashboard as well as through our&nbsp; [Custom Reports](/user-guide/measurement/campaign-reporting/custom-reports/)tool. We can now report conversion metrics (ie. impressions conversions, view conversions, click conversions) by conversion pixel allowing you to distinguish which conversion pixel (action) drove the most conversions.

A conversion pixel is a piece of code that's put on a website (often ad advertiser's landing page, but possibly a publisher) to track a certain post-ad experience action.&nbsp;&nbsp;For example, registering as a Facebook fan, filling out a form, buying a product, etc.&nbsp;&nbsp;The conversion action is completely up to the advertiser and how they implement the pixel on their site.
In the display world, conversion pixels typically track:

* Click-through - User clicked on the ad to get to the conversion site
* View-through - User viewed an ad and went to the conversion site sometime later

For reference, here's DFAs docs on what they support:&nbsp;

[http://www.google.com/support/dfa/partner/bin/static.py?page=guide.cs&guide=28818&topic=28831&printable=1](http://www.google.com/support/dfa/partner/bin/static.py?page=guide.cs&guide=28818&topic=28831&printable=1)
However, in our video world, we support the following

* Click conversion - User clicked on the ad and either directly landed on the conversion page, or converted sometime later
* View conversion - User viewed the video and went to the conversion page sometime later
* Impression conversion - User was exposed to an in-banner impression and went to the conversion page sometime later

Note that a view conversion in our system is not quite the same thing as a "view-through" conversion in the display world.

Conversion pixels also support the notion of a "lookback window". &nbsp;This defines the trailing time period for which the original activity with the ad will be considered eligible for conversion. &nbsp;By default, all conversion types have a lookback window of 30 days. &nbsp;That means that if the ad was seen 40 days ago before the conversion page was hit, it would not be considered a valid conversion and wouldn't be counted.
Conversions can be any action performed by a viewer who was exposed to an ad such as returning to the brand site, signing up for a newsletter, inquiring for more information, etc.&nbsp;&nbsp;It is recommended to&nbsp; [create a conversion pixel](../../../../user-guide/execution/placement-setup/conversions/conversion-pixel-setup.md)at least a week prior to campaign launch to ensure proper implementation and pixel firing. Once implemented, enable the conversion pixel in a particular placement.
**&nbsp;** 