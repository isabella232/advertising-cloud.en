---
title: Advertiser Account Settings
description: Advertiser Account Settings
---

# Advertiser Account Settings

*Not Available to Read-only Users*

## General Settings

**Advertiser Name:** The advertiser name.

**Category:** The category in which the advertiser’s business operates. The category will be communicated to the publishers when you bid on inventory. Make sure you choose a category that aligns with your ads, or publishers may reject your ads.

>[!NOTE]
>
>If you select *Other*, the advertiser won't be able to access DSP On Demand Inventory.

**Advertiser URL:** The advertiser’s homepage or main website URL (beginning with http:// or https://).

**Share all private exchange feeds into this advertiser:** (New advertiser accounts only) Makes all private exchange feeds configured for the organization's DSP account available to the advertiser.

### Adobe IMS IDs

Advertisers with additional Adobe Experience Cloud products can share data across some products using the company's unique Organization ID for Experience Cloud. You can configure specific product integrations in the Integrations section.

**Account IMS org and ID:** (Advertisers with additional Experience Cloud products that are licensed through an Experience Cloud account with multiple advertisers; optional) The account's Experience Cloud Organization ID.

**Advertiser IMS org and ID:** (Advertisers with direct licenses for additional Experience Cloud products; optional) The advertiser's Experience Cloud Organization ID.

### Integrations

(Optional) Additional Experience Cloud products linked to the DSP account. The products must be associated with the same Experience Cloud Organization ID provided in the Adobe IMS IDs section.

**Adobe Media Optimizer:** (Advertisers with Advertising Cloud Search or who use Advertising Cloud conversion pixels) A Search account with which DSP will exchange attribution data.

**Adobe Device Co-op or 3rd Party Graph:** (Advertisers who use Advertising Cloud conversion pixels; optional) You can leverage a device graph for person-based attribution measurement from the advertiser's account settings in Advertising Cloud Search.

>[!NOTE]
>
> * Device attribution is available only for conversions tracked using the Advertising Cloud conversion tracking service, not conversions tracked by Adobe Analytics.
> * You can also select a person-based device graph for cross-device targeting and frequency management at the [campaign level](/help/dsp/campaign-management/campaigns/campaign-settings.md). You can then set up cross-device targeting at the [placement level](/help/dsp/campaign-management/placements/placement-settings.md) and further frequency caps at the [package level](/help/dsp/campaign-management/packages/package-settings.md) and [placement level](/help/dsp/campaign-management/placements/placement-settings.md). Cross-device targeting and frequency management don't require advertiser-level attribution measurement; instead, they work with the device graph that's specified in the campaign settings.

**Adobe Analytics:** (Advertisers with Adobe Analytics; optional; applicable only to data collected using Advertising Cloud conversion tracking tags that include an EF Redirect and token only) One or more Analytics report suites to which DSP will send data it collects from publishers and supply side partners. Analytics will also send the data it collects from the client’s site to DSP.

For the data to appear in the report suites, the Search advertiser-level setting to "Enable tracking for SAINT feeds" must be enabled. In addition, the advertiser's Analytics account must be configured to receive data from DSP. <!-- from DSP or Advertising Cloud? -->

>[!WARNING]
>
>If you remove a previously linked report suite, DSP will no longer exchange data with that suite. Expect to see data fluctuations. <!-- Fluctuations where? Clarify -->

**Adobe Analytics Cloud:** (Advertisers with Adobe Audience Manager or Adobe Analytics; optional) An Audience Manager or Analytics account from which DSP will pull in segment metadata, hierarchy data, and unique audience data for all of the advertiser's Adobe audiences. This includes data for:

* Audience Manager segments
* Analytics segments that are published to Adobe Experience Cloud
* Segments that are created in Adobe Experience Cloud using the People core service
* Segments that are created in Adobe Experience Platform and sent to Advertising Cloud via Audience Manager

The initial sync takes about 24 hours. After that, data is synced in real time, with a one- to two- second delay. Segment membership data is sent to Advertising Cloud only after one of the following:

* The segment is targeted in an Advertising Cloud placement or audience library
* The segment is added to the Advertising Cloud batch and real-time destinations within the Audience Manager user interface

## Targeting Settings

You can optionally configure default targets for the advertiser's new placements. Users can override the default targets for any new placement.

### Geo-targeting

**Countries** – The default country for each placement’s geo-targeting. Users can change the country, and configure more specific geo-targeting, for each placement.

### Audience Targeting

**Audiences to exclude:** Any audiences or segments that will be suppressed by default. Users can change the exclusions for each placement.

### Media Quality

#### Contextual Filtering

Types of Comscore, DoubleVerify, Integral Ad Science, and Peer39 contextual filters to apply. You can override the advertiser-level settings at the [placement level](/help/dsp/campaign-management/placements/placement-settings.md).

##### DoubleVerify

**Block sites that are:** (Optional) One or more types of inventory context to block by default. Additional fees may apply.

##### Peer 39

**Target sites that are:** (Optional) One or more types of inventory attributes to target by default. Additional fees may apply.

##### ComScore

**Block sites that are:** (Optional) One or more types of inventory attributes to block by default. Additional fees may apply.

##### Integral Ad Science

**Adult Content:** (Optional) The degree of adult content for which to block ads by default: *Do Not Block* (the default), *Standard*, or *Strict*. Additional fees may apply.

**Alcohol Content:** (Optional) The degree of alcohol content for which to block ads by default: *Do Not Block* (the default), *Standard*, or *Strict*. Additional fees may apply.

#### Pre-Bid Fraud Blocking

Types of sites to block based on fraudulent traffic and suspicious activities measured through DoubleVerify, Integral Ad Science, and Peer39. You can override the advertiser-level settings at the [placement level](/help/dsp/campaign-management/placements/placement-settings.md).


##### DoubleVerify

**Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices:** By default, blocks all 100% invalid traffic, including traffic on highjacked devices, for new placements. Additional fees may apply.

**Also block sites with:** (Optional) An additional level of fraud and invalid traffic that will cause DSP to block ads by default:  *None* (the default, which doesn't block additional traffic), *>2% Average Fraud/IVT levels (lowest reach)*, *>4% Average Fraud/IVT levels*, *>6% Average Fraud/IVT levels*, *>10% Average Fraud/IVT levels*, or *>25% Average Fraud/IVT levels*. Additional fees may apply.

##### Peer 39

**Block sites that are:** (Optional) One or more types of fraud that will cause DSP to block ads by default: *Fraud* (which blocks all sites with fraud), *Fraud: Bot Sites_Non-Human traffic*, and/or *Fraud: Zero Ads*. Additional fees may apply.

##### Integral Ad Science

**Block sites that are:** (Optional) A type of suspicious website or app activity that will cause DSP to block ads by default: *None* (the default, which doesn't block ads based on suspicious activity), *Suspicious Activity - High Risk*, or *Suspicious Activity - High or Moderate Risk*. Additional fees may apply.

#### Ads.text

**Ads.txt Filtering:**
By default, which level of [Ads.txt](https://iabtechlab.com/ads-txt-about/) pre-bid filtering to use by leveraging each publisher's Authorized Digital Sellers list:
* *Opt out of ads.txt (default)*: To buy inventory from all sellers.
* *Ads.txt sellers + sites without ads.txt*: To prioritize buying inventory from a domain's authorized direct sellers and resellers.
* *Ads.txt sellers only*: To buy inventory only from a domain's authorized direct sellers and resellers.
* *Ads.txt sellers only*: To buy inventory only from a domain's authorized direct sellers.

You can override the advertiser-level setting at the [placement level](/help/dsp/campaign-management/placements/placement-settings.md).

#### Safe Site Block

**Enable Site Safety Block:** By default, enables a real-time, post-bid filter to ensure that ads serve on the sites that the advertiser is targeting. <!-- Can remove this: Users can enable or disable the feature for each placement. I don't see this option, but I should probably verify. If this can't be edited at placement level, then remove "By default." If it can, say that you can override at placement level. -->

#### DoubleVerify Authentic Brand Safety

**DoubleVerify Account:** (DoubleVerify customers only; optional) The brand safety segment ID associated with the organization's DoubleVerify account.

**Enable Authentic Brand Safety:** (Optional) By default, enables DoubleVerify Authentic Brand Safety, which blocks impressions post-bid using the custom brand safety rules configured for the specified segment ID. DSP bills your account for usage for the segment ID.

You can override the advertiser-level setting at the placement level.

<!--
>[!MORELIKETHIS]
>
>* [Create an Advertiser Account](/help/dsp/admin/advertiser-create.md)
>* [View the Advertiser List for the Account](/help/dsp/admin/advertiser-view.md)
-->
