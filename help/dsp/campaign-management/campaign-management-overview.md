---
title: Overview of Campaign Management in Advertising Cloud DSP
description: Learn about the campaign management hierarchy and components.
feature: Packages, Placements, Ads, Creatives
exl-id: c94e08d0-0dd5-4cf9-8df2-9eb4c591375c
---
# Overview of Campaign Management in Advertising Cloud DSP

Advertising Cloud DSP campaigns have the following hierarchy:

* Campaign
  * Package(s)
    * Placement(s)
      * Ad(s)
        * Creative(s)
<!-- Do clients think in terms of insertion orders? If yes, then work in the following info.:
In Advertising Cloud DSP, an insertion order is represented as a campaign, and line items are represented as packages. Each package will include placements, which can use different strategies and tactics to deliver the line item requirements.
-->

## Campaigns

[Campaigns](/help/dsp/campaign-management/campaigns/campaign-about.md) are the overarching framework of flight settings. Each campaign is configured with an advertiser, start and end dates, an overall budget, a cross-device targeting option and default frequency cap, and reporting options for viewability, fraud, brand safety, and audience verification. All campaign-level settings automatically apply to each package and placement within the campaign.

## Packages

Each campaign can contain one or more [packages](/help/dsp/campaign-management/packages/package-about.md), each of which includes a set of placements.

Use packages to group placements for delivery to a set budget, performance goal, and custom pacing strategy. DSP optimizes packages by shifting budgets to the best-performing placements in the package. You can organize packages by placement format, inventory type, data provider, persona, or other distinguishable characteristics.

Packages are optional but recommended.

## Placements

A [placement](/help/dsp/campaign-management/placements/placement-about.md) stores targeting parameters for one or more ads of the same ad type. You can create a placement for a single campaign or package, and then assign ads to it.

## Ads

[Ads](/help/dsp/campaign-management/ads/ad-about.md) include creative assets and tracking URLs. You can either upload your creative assets and DSP will serve the ads that use them for free, or you can upload third-party ad serving tags.

Once your ads are set up, you'll need to attach each ad to a placement. You can attach a single ad to one or more placements.

All active, approved ads in an active placement in an active campaign are eligible to run based on the placement targeting parameters.

## Creatives

You can upload audio and video files to use in ads for specified campaigns.
<!-- add link to [About Creative Management](/help/dsp/campaign-management/creatives/creative-about.md) when it's available-->

You can immediately create an ad with the uploaded creative, or you can create an ad later from either the Creatives view or the Ads view.

>[!MORELIKETHIS]
>
>* [About Campaign Management](/help/dsp/campaign-management/campaigns/campaign-about.md)
>* [About Package Management](/help/dsp/campaign-management/packages/package-about.md)
>* [About Placement Management](/help/dsp/campaign-management/placements/placement-about.md)
>* [About Ad Management](/help/dsp/campaign-management/ads/ad-about.md)
>* [Campaign Launch Checklist](/help/dsp/campaign-management/campaign-launch-checklist.md)
>* [Best Practices for Setting up Performance Campaigns](/help/dsp/optimization/campaign-best-practices-performance.md)
>* [About In-Platform Reports](/help/dsp/campaign-management/reports/campaign-reports-about.md)
>* [About the Campaign Data Views](/help/dsp/campaign-management/reports/campaign-data-views-about.md)
