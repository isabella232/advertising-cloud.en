---
edit-last: 3
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
pubDate: Fri, 04 Jul 2014 16:12:33 +0000
dc-creator: hchang@adobe.com
guid: https://education.tubemogul.com/userguide/?page_id=1537
isPermaLink: false
description: 
postId: 1537
postDate: 2014-07-04 08:12:33
postDateGmt: 2014-07-04 16:12:33
commentStatus: open
pingStatus: open
postName: feed-management
status: publish
postParent: 1535
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Feed Management {#feed-management}

You can manage your feeds from the DSP > Private Inventory > Analytics view. This view groups your feeds by publisher name and includes metrics on feed delivery and performance and also warns you of feeds potentially serving blank impressions or without activity. Below are definitions of some of the key metrics. You can filter the list by additional metrics at the site level.

* **Auctions**: The number of auctions we have observed for the feed – this represents the number of opportunities we saw to buy inventory on this feed, and it’s shown as an integer.
* **Bid rate**: The percentage of auctions where a bid was submitted for this particular feed – this is shown as a percentage, and is calculated as bids divided by auctions.
* **Win rate**:  A win is an impression that you bid on successfully. The win rate is the percentage of auctions where the impression was won in this feed  - this is shown as a percentage, and is calculated as impressions/bids.
* **Red** means the feed requires immediate attention most likely because there is no activity on the feed or a default ad is missing from a guaranteed feed.
* **Orange** means the feed will need attention soon most likely because an ad flight is ending within 4 days.
* **Progress bar**: Will only show up if you filled out the optional 'Tracking" section of the [BrandAccess Feed Creation](../../../../dsp/planning/private-inventory/brandaccess.md) modal. The purple bar indicates actual budget spent vs. desired spend. Blue bars indicate impressions delivered vs goal.

![Feed troubleshooting](assets/feed-troubleshooting.png)

## Available options
The following options are available for any feed from the gear icon in the right column.

* **Edit** the feed details.
  >[!NOTE]
  >
  >Any changes to the Duration, Ad Server, or choice of Guaranteed/Non-Guaranteed options will change the tag structure, and you'll need to send the new tag to the publisher to replace the existing tag.

      * If you are making a non-guaranteed feed into a guaranteed feed, you will need to choose a default ad, and the system will create a placement for you.
      * If you are making a guaranteed feed into a non-guaranteed feed, you should pause the guaranteed placement and default ad.
      * If you are making either a "guaranteed" or "non-guaranteed" change, we recommend creating a new tag and archiving outdated tags.

    * If you need to change the billing method &mdash; from directly from the publisher to from Advertising Cloud, or vice versa &mdash; contact your Account Manager to assist with the transition.

* **Attach an ad** &mdash; (Guaranteed feeds only) Attach default ads for the feed.
* **Archive** &mdash; Move the feed to the Archived Feeds section. Archiving a feed won't stop traffic from running on the feed.
* **Show Pixels** &mdash; Generate an event pixel for the tag. 
* **Placements and Ads** &mdash; View a list of placements and ads that target the feed so you can verify if the feed is set up properly and receiving inventory. This page uses the same orange and red indicators as the main Private Inventory feed management page.
* [See Report](/help/dsp/planning/private-inventory/feeds-reporting.md) &mdash; Open the feed details, which are also available by clicking the feed name.
