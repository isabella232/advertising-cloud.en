---
title: About Private Inventory
description: About Private Inventory
---
# About Private Inventory

<!-- Can any of these include premium inventory? I think Deal Id Inbox offers only non-premium inventory? -->

Private exchanges allow publishers to create exclusive pools of video inventory, which approved advertisers can use to buy via real-time platforms. A private exchange offers the confidence of a direct buy combined with programmatic benefits like efficiency, streamlined workflow, and centralized campaign analytics.

If you have direct relationships with publishers, you can streamline your media buying process and workflow by using your own private deals in your Advertising Cloud DSP placements. Advertising Cloud DSP will integrate with all of your publishers when you set up an account. If you want access to additional publishers later, contact your Adobe account manager to set up access. <!-- + sentence from Ramey about how we certify the publishers -->

You can use each private deal as a placement target for multiple campaigns across specified advertisers. <!-- verify true for all -->

## Ways to Set up Private Deals

### Deal IDs  <!-- naming??? -->

All of your private deals with a deal ID are financed and invoiced by Adobe.

<!-- replacement for "deal ID" option in smart ad serving -->

* (Optional feature that requires activation) From the Deal ID Inbox, you can review and quickly accept your agreed-upon, guaranteed and non-guaranteed private inventory deals from publishers on the following supply-side platforms (SSPs): Google Authorized Buyers (formerly known as AdX), FreeWheel, and Rubicon. Accepting a deal automatically pre-populates a new Deal ID record with details from the publisher, and you need to enter only the publisher <!-- always? or just in some cases? -->, the media type, who can access the deal, and any labels to apply to the deal so it's easy to find. <!-- are labels a dimension you can report on? --> <!-- Are these deals they've already started negotiating outside of our UI, or are they being offered only in our UI? -->

   For each available deal, you can review the deal details sent directly from the publisher. Some deals are grouped as proposals (packages), and you can see the individual deal details by reviewing the deal.
   
   You can accept any available deal or move an incorrect deal to the Ignored Deals tab. You can also un-ignore deals, which moves them back to the New Deals tab so you can potentially accept them.
     
   The Deal ID Inbox is refreshed hourly, and you can manually refresh the list with any new deals that are available at any time.

   For each deal, you can select one publisher and one media type (Desktop Video, Mobile Video, Connected TV, Display, or Audio), and you can share the deal with specific advertisers and with all advertisers for a specific account.

   To activate this feature for any of the available SSPs, contact your Adobe account manager.

   <!-- more info at https://wiki.corp.adobe.com/display/TMCS/Deal+ID+inbox#DealIDinbox-WhatisdealIDinbox? -->

* You can manually set up information about a private deal you've already negotiated.

   Advertising Cloud DSP can integrate with all of your publishers when you set up an account. If you want access to additional publishers later, contact your Adobe account manager to set up access.

   All of your private deals with a deal ID are financed and invoiced by Adobe.

   You can share each deal with multiple advertisers in the account, and you can use the deal as a placement target for multiple campaigns. For guaranteed deals, you must create a default placement after creating the deal, but you can add the same deal to additional placements to ignore the default placement.

### Smart Ad Serving (renamed "VAST Tags" or such?)

<!-- From Ashley:  we will remove the "are you using a deal ID" option and we'll rename the "Smart ad serving" option, likely to be "vast tags" or something. We will also move the new deal ID form selection to be the first item to select, vs at the bottom of the selection UI.>

<!-- VAST third-party ad tags only (digital Video Ad Serving Template) -- no more deal IDs. Are we going to rename this UI/feature accordingly? -->

Smart Ad Serving provides RTB-powered decisioning and execution <!-- (and optimization, supposedly -- to maximize the value of each impression, as well as cap frequency - but is this in some way diff. than the package/placement optimization/placement capping? --> for publisher direct deals for third-party VAST tags. <!-- wording??? --> It allows advertisers with existing private deals to activate their inventory for centralized planning, buying, and measurement in Advertising Cloud DSP.

You can share each deal with multiple advertisers in the account, and you can use the deal as a placement target for multiple campaigns. For guaranteed deals, you must create a default placement after creating the deal, but you can add the same deal to additional placements to ignore the default placement.

<!-- (Training video at https://education.tubemogul.com/videos/inventory-setting-up-pmps/says we can help with issues. Do we provide services to resolve issues with smart ad serving deals that we don't for simple ad serving or Deal IDs? For managed clients only, or for self-service clients too? -->

Smart ad serving is available for the following types of inventory:

* desktop video
* mobile video
* connected TV video
* audio

### Simple Ad Serving

Simple Ad Serving provides non-decisioned, guaranteed ad delivery and reporting for a specified publisher and a single ad type using a single, dedicated placement. <!-- wording? -->

Simple ad serving is available for the following types of inventory:

When the ad source is Ad Serve (an ad tag) <!-- "When Advertising Cloud DSP or a third-party ad server will serve the ad and Advertising Cloud will provide an ad tag to send to the publisher"? -->:

* desktop video
* tablet and mobile video
* connected TV video
* standard display on desktop, tablet, and mobile
* interstitial display on mobile

When the ad source is Site Serve (an event pixel) <!-- "When the ad will be served directly by the publisher (site serve) and Advertising Cloud will provide an event tracking pixel to send to the publisher"? -->:

* desktop standard pre-roll
* tablet and mobile standard pre-roll
* connected TV standard pre-roll

You can create a simple ad serving deal in the Inventory > Deals view. Advertising Cloud automatically generates a placement for the ad, targeting the deal but without the option for additional targeting, budget, or frequency capping.






<!-- old UI -- see if these still exist in the latest and update/reorg all as needed -->

#---
title: Deal Reporting
description: Deal Reporting
---
# Deal Reporting

On the main feed management page at DSP > Private Inventory > Analytics, you can access more than 30 metrics, ranging from impressions and costs, to completion rates and click throughs to conversions, broken out by publisher and feed.

<!-- screen shot -->

The metrics you see onscreen and in downloaded reports are for the specified date range. To change the metrics displayed onscreen, click the metric list icon next to the Options column on the top right. To see all metrics at once, you can download all of the data for the active and archived feeds sections as a Microsoft Excel spreadsheet.

<!-- screen shot -->

## Deal Details

At the individual feed level, click the gear icon and then select “See Report” to see detailed data. The data includes all of the same metrics as you could from the Private Inventory Analytics page, but you can also view and export reporting by Advertiser, Campaign, Ad Type, and Site. You can also get private feed reporting via custom reports.

<!-- screen shot -->
