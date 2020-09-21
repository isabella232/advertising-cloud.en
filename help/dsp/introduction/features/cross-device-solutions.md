---
title: Cross-Device Solutions
description: Cross-Device Solutions
---
# Cross-Device Solutions

Advertising Cloud DSP integrations with LiveRamp and Adobe Device Co-op allow you to extend your audience to all of a person's known devices, not just the devices your brand has tracked. The integrations also provide frequency capping and attribution measurement across all devices.

When you use a supported people-based device graph, you can:

* Match audiences across channels and devices to deliver ads to people and households, rather than to devices.
* Balance ad exposure by understanding and capping frequency across individuals.
* Test strategies that expose vs. convert audiences across channels or devices.

## Benefits of Each Device Graph

* Adobe Device Co-op:
    * Provides an opt-in pool of participating Adobe advertisers’ deterministic and probabilistic data
    * Provides strong cookie ID connections powered by desktop and mobile web visitors
    * Includes data predominantly from the United States and Canada
    * Has no usage fees

* LiveRamp device graph:
    * Provides a deterministic data pool, including offline customer data
    * Provides even coverage between cookie IDs and mobile device IDs
    * Includes data predominantly from the United States
    * Is free for frequency capping and attribution measurement
    * Priced at $0.35 CPM for extended impressions (impressions that are delivered solely by using the LiveRamp device graph rather than on devices found within the targeted audience segments)

       The rate is reflected on your account rate card.

## People-Based Frequency Management

People-based frequency management allows you to specify frequency caps at the person level, rather than the device level, for true media exposure control.

### Activate People-Based Frequency Management

* **Campaigns:** When you create a new campaign, you can specify a Cross-Device Level setting. Enable “Same Device” -> “People,” and select a device graph. The specified device graph is used for both cross-device targeting at the placement level and for people-based frequency management at the campaign, package, and placement level. Frequency caps apply across all of a person's known devices.

 For more information, see [Campaign Settings](/help/dsp/campaign-management/campaigns/campaign-settings.md).

   Once you save a campaign, you can't change its Cross Device Level setting.

* **Packages:**  You can optionally set additional frequency caps at the package level. DSP will respect the strictest frequency cap in the campaign hierarchy.

* **Placements:** You can optionally set additional frequency caps at the placement level. DSP will respect the strictest frequency cap in the campaign hierarchy.

## People-Based Targeting

People-based targeting allows you to find customers across desktop and mobile.

### Activate People-Based Targeting

* **Campaigns:** When you create a new campaign, you can specify a Cross-Device Level setting. Enable “Same Device” -> “People,” and select a device graph. The specified device graph is used for both cross-device targeting at the placement level and for people-based frequency management.

 For more information, see [Campaign Settings](/help/dsp/campaign-management/campaigns/campaign-settings.md).

* **Placements:** When you select audience targets for a placement in a campaign with a specified device graph, a Cross-Device Targeting option allows you to extend your targeting across all of a person's known devices (per the device graph specified in the campaign settings), even devices that aren't in the specified segments.

### Set Up Reporting for People-Based Targeting

You can include the following metrics in custom reports:

* **Extended Impressions:** (In the Build Your Report section under Metrics > Std. Metrics) The volume of incremental impressions delivered by leveraging a device graph (and not found within the original audience segments). This metric is also used to calculate applicable fees associated with using a third-party device graph.

   To determine the cost of your extended impressions during a time period, run a custom report that includes the "Extended Impressions" column, and then multiply the total number of extended impressions by $0.00035 ($0.35/1000 impressions).
   
   The aggregated cost is also included in the column "Billable Other Net Spend” (under Metrics > Spend), although that metric also includes other campaign fees you may have added.

* **Device Graph:** (In the Build Your Report section under Dimensions > Campaign) The selected device graph for a particular campaign, package, or placement.

## People-Based Attribution Measurement

*Advertisers with Advertising Cloud Conversion Tracking Only*

With people-based attribution, you can attribute conversions that took place on a different device than the device on which the media exposure occurred. People-based attribution measurement is available across DSP, Search, and Creative for advertisers who have implemented Advertising Cloud conversion pixels on their sites.

### Enable People-Based Attribution Measurement

If you would like to activate cross-device attribution measurement, contact your Adobe account manager. For Adobe Device Co-op accounts, you'll need to provide your signed Adobe Device Co-op contract and Experience Cloud Organization ID (formerly called IMS org ID).

To see if an advertiser account is configured to use a device graph for attribution measurement:

1. In the main menu, click **Settings > Advertiser**.
1. Hold the cursor over the advertiser row and click **Edit**.
1. In the Integrations section of the advertiser settings, see if the Cross-Device Attribution setting is active.

   For active integrations, the device graph is indicated.

### Set Up Conversion Reports for Cross-Device Conversion Attribution

#### Conversion Report Settings

When a device graph is enabled for attribution measurement, the Conversion Report includes a "Cross-Device Breakout" setting, which allows you to include up to three separate columns for each conversion metric, including:

* <*Conversion*>(tp): Includes the total conversions (total people), which includes both same-device conversions and cross-device conversions (if applicable). In the report, "(tp)" is appended to the conversion metric name, rule type, and conversion types in the conversion path (for example, "Responses(le)(tl)(tp)).

* <*Conversion*>(sd): (Optional) Includes only conversions for which only a single device was tracked in the conversion path. In the report, "(sd)" is appended to the conversion metric name, rule type, and conversion types in the conversion path (for example, "Responses(le)(tl)(sd)).

* <*Conversion*>(xd): (Optional) Includes only conversions for which more than one device was tracked in the conversion path. In the report, "(xd)" is appended to the conversion metric name, rule type, and conversion types in the conversion path (for example, "Responses(le)(tl)(xd)).

#### How to Interpret the Conversion Report

If you sort the percentage of total conversions that are cross-device ((xd)/(tl)) from high to low, you'll understand what is driving above-average cross-device conversions. You can use this to inform your creative or targeting strategy to match messaging and channel investment to user behavior.

* Packages – See which packages drive the most total conversions, and which ones have a high percentage of cross-device conversions. This can help you understand where to focus spend.

* Placements – Compare placement performance and attribution (for example, a mobile web ad may drive conversions on desktop). Without a device graph for attribution, you may miss a mobile web placement’s impact on desktop conversions, or it may be buried if the majority of your users convert on desktop and not mobile web.

* Ads – Discover which ads drive higher conversions, and quantify their value and impact across both web browsers and mobile app environments.

* Sites – Optimize across sites rather than manually excluding sites completely. If a website drives cross-device conversions, then you can see on which devices this behavior occurs.

* Deals – Improve manual optimization by verifying which inventory deals deliver cross-device conversions, and then deciding if you should expand your targeting to include more devices and channels in those deals.

>[!MORELIKETHIS]
>
>* [Report Settings](/help/dsp/reports/report-settings-custom.md)
>* [Campaign Settings](/help/dsp/campaign-management/campaigns/campaign-settings.md)
>* [Package Settings](/help/dsp/campaign-management/packages/package-settings.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
