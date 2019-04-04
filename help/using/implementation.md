---
title: Overview of implementing Advertising Cloud Creative
description: Overview of implementing Adobe Advertising Cloud Creative
seo-title: Overview of implementing Advertising Cloud Creative
seo-description: Overview of implementing Advertising Cloud Creative
---

# Overview of Implementing Adobe Advertising Cloud Creative

The Advertising Cloud Creative operations team will work with each advertiser to set up its creatives and creative experiences, either implementing the ad experiences as ads within your DSP or providing your team with the third-party ad tags to implement themselves, and validating the initial cost, click, and conversion data.

On an on-going basis, the Advertising Cloud Creative account management team, the agency team, or the advertiser (depending on the terms of the service level agreement) will need to monitor each experience and to edit it as necessary to meet the advertiser's goals.

## Initial Setup Tasks for Advertising Cloud Creative Campaigns

The implementation team and/or your agency will work with you do the following:

1. Define your personalization goals (such as whether you'll personalize ads for prospecting or retargeting); all first-, second-, and third-party data that's available, including creative assets, audience segments, and CRM data; and your strategy for achieving your goals.
1. *New advertiser accounts* - Set up administrative accounts:
   1. Set up the advertiser's account for Advertising Cloud Creative, and also create an account in Advertising Cloud Search.
      The Advertising Cloud Creative account setup is within Advertising Cloud DSP, even if the advertiser isn't a DSP customer.
      Similarly, even if the advertiser isn't a Search customer, the Search account is used to create conversion tracking tags and set up conversion columns in Advertising Cloud Creative.
   1. (If necessary) Create user accounts for the advertiser to view and manage its creatives and ad experiences and to generate reports.
1. *Optional* - If you want to create first-party audience segments to include as targets for your creatives, then create the tags in either of the following ways:
   * Create retargeting pixels to retarget ads to visitors with specific attributes to specific landing pages or conversion pages, and then generate tags to insert in the relevant web pages.
   * *Advertisers with Advertising Cloud DSP* - Within Advertising Cloud DSP, create audience segments to track all visitors to specific landing pages or conversion pages, and then generate tags to insert in the relevant web pages.
     Both types of tags are image tags, which display a 1-pixel x 1-pixel transparent image (pixel), which is invisible to end users, on the web page on which they are added. Later, you can configure creatives in an ad experience to target or segments, so that the relevant ad elements are displayed only to users who previously visited site pages associated with the segment.
     The advertiser's IT department or other group may need to schedule, or be informed about, the tag deployment.

     >[!NOTE]
     >
     >You can also use your first-party audiences from Adobe Audience Manager and Adobe Analytics as creative targets. 

1. Set up ad experiences based on your advertising goals:
   1. *Advertisers with Adobe Experience Manager; optional* Configure access to image assets in the Experience Manager account.
   1. Set up creatives to use in your experiences:
      * For creatives that Advertising Cloud Creative will host, upload them.
      * For creatives hosted on a supported third-party ad server, point to the creative files.
    1. Sequence ad targets and corresponding creatives as ad experiences.
    Ad targets can include retargeting pixels that you create in Advertising Cloud Creative; your audience segments in Adobe Experience Cloud (including in Advertising Cloud DSP, Audience Manager, or Analytics); geographic targets; or specific data triggers on the web page (such as `SKU=01234567890123` or `Cart=empty`).
1. Set up conversion tracking for your ad experiences:
   1. Set up conversion tracking. Depending on the implementation, this may involve adding conversion tracking tags to the advertiser's web pages and/or setting up a daily feed drop for conversion data that the advertiser has collected separately.
      You can generate Advertising Cloud conversion tracking tags within Advertising Cloud Search or within Adobe Dynamic Tag Manager (formerly called Dynamic Tag Manager).  Note:  You must use JavaScript conversion tags, not image tags.
      The advertiser's IT department or other group may need to schedule, or be informed about, the tag deployment.
   1. (Optional) Within Advertising Cloud Search, make each conversion (transaction property) available as an individual column set in data views and reports.
   A conversion (transaction property) is listed in Advertising Cloud Search after at least one conversion event has been tracked.
   If you don't make specific metrics available, then all conversions are consolidated in one "Conversions" column set.
   1. Validate the data that is tracked.
1. (Optional) Set up delivery of scheduled reports to specified email addresses.
   For instructions, see the help chapter on "Reports."
1. Set up ad campaigns on Advertising Cloud DSP or another DSP, and provide JavaScript or iframe tags for the ad experiences to the advertiser, who can implement them as third-party ads in the DSP.
1. Monitor the performance of your completed ad experiences, either viewing predefined performance details for individual experiences or creating custom performance reports.
