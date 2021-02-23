---
title: Placement Settings
description: Placement Settings
---

# Placement Settings

## Basics

**Placement name** The placement name.

>[!TIP]
>Use a naming convention that makes sense for your situation. One suggested naming convention is "*\<Campaign Name\>: \<Ad Unit\>: \<Duration\>: \<Targeting\>*."

**Status:** The placement status: *Active* (the default) or *Paused*.

>[!TIP]
>The best practice is to pause the placement until you're ready to launch it.

**Details:** (Read-only) The applicable ad type, the account that is creating or created the placement, and the parent campaign. To see more details, click **Show more**.

**Templates:** Opens a list of existing placement templates. To auto-populate targeting settings from a template:

1. Do either of the following:

   * To reuse all target from a template, select the check box next to the template name.
   
   * To reuse individual target types from a template, expand the template name and select the check box next to  the target types you want to reuse.

1. Click **Apply**.

**Ad specs for forecast:** (Video ad formats only) The ad duration and/or ad specifications, which are used to calculate the Forecast projection on the right. The fields vary by ad type.

**Placement tags:** (Optional) Keywords or nicknames to help you locate this placement.

## Goals

**Package:** (Optional) A package to which the placement is assigned. Click ![Edit](/help/dsp/assets/edit.png) to select and existing package or create a new package. When you assign the placement to a package, the Goals section is updated with the flight dates, delivery goal, and budget from the package.

**Flight Dates:** The start date and end date for the placement. Approved ads are eligible to run during the flight when the placement is active and assigned to an active package or campaign.

The dates for the package (when applicable) or campaign are auto-populated by default.

>[!NOTE]
>
>* The flight dates must be included within the campaign flight dates and the package flight dates.

### Placements Assigned to Packages with Package-level Pacing

**Placement Funding:** How to budget for the placement:

* *Optimize based on performance:* Controls the budget at the package level.
* *Set a fixed budget cap:* Allows you to set a daily, weekly, monthly or all-time placement budget. Enter a value and the duration (*All time*, *Daily*, *Weekly*, *Monthly*).

**Max Bid:** The maximum to pay for 1000 impressions.

**Placement Pre-bid Filters:** Up to five KPI thresholds (such as a minimum viewability metric or click-through rate) that must be met for bidding to occur. You can use pre-bid filters as optimization tactics, but understand that each rule may limit the opportunities on which this placement can bid. To add or edit filters:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Do either of the following:
   * To add a filter:
      1. Click **Add Filter**.
      1. Next to **Only bid if**, select a metric, and then enter a value.
   * To remove a filter, click **X** in the filter row.
1. Click **Save**.

 See descriptions of each pre-bid filter at [Placement-level Pre-Bid Filters and How to Use Them](/help/dsp/optimization/optimization-pre-bid-filters.md).

### All Other Placements

**Budget Goal:** The gross budget cap and the budget interval (*All time*, *Daily*, *Weekly*, *Monthly*).

**Gross Budget Goal:** (Placements in campaigns with margin management only) The gross budget cap and the budget interval (*All time*, *Daily*, *Weekly*, *Monthly*).

**Optimization Goal:**  The optimization goal for the package. See descriptions of each optimization goal at [Optimization Goals and How to Use Them](/help/dsp/optimization/optimization-goals.md).

**Target Goal:** The target goal, which is used to track performance.

>[!NOTE]
>
>This field is only a benchmark and isn't used for decisioning.

**Pace on:** What pacing will be based on:

* **Budget goal:** (Default) This option delivers as many impressions as possible within the allocated budget.

* **Impressions:** This option delivers impressions until a specified quantity is reached within a specified interval. When you select this option, specify the number of impressions and the interval: *All time,* *Daily,* *Monthly,* or *Weekly*.

**Max Bid:** The maximum to pay for 1000 impressions.

**Pacing Fill Strategy:** (Packages with package-level pacing only) How to pace ad delivery:

* *Even:* (The default) Paces delivery uniformly throughout each flight, with a target of 50% of the delivery in the first half of the flight.

* *Frontload:* Accelerates delivery so that it is 65-75% complete halfway through the flight.

* *Aggressive Frontload:* Accelerates delivery so that it is 75-85% complete halfway through the flight.

**Placement Pre-bid Filters:** (Optional) Up to five filters that must be met for bidding to occur. You can use pre-bid filters as optimization tactics, but keep in mind that each rule may limit the opportunities on which this placement can bid. To add or edit filters:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Do either of the following:
   * To add a filter:
      1. Click **Add Filter**.
      1. Next to **Only bid if**, select a metric, and then enter a value.
   * To remove a filter, click **X** in the filter row.
1. Click **Save**.

## Geo-Targeting

**Audience Location:** (Optional) Specific locations in which to include or exclude ads in the placement. If you don't specify any locations, all locations are targeted.

>[!NOTE]
>
>City and DMA locations aren't available for Roku placements.

To specify locations:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Do any of the following:
   * To include or exclude a Country, State, City, DMA, Federal Legislative District, or State Legislative District:
      1. Select the location type in the left column.
      1. (As needed) Click a location to expand it.
      1. Next to the location, click *Include* to include it as a target or *Exclude* to exclude it as a target.
   * To search for a postal code and include or exclude all selected results:
      1. Click Search Postal Code.
      1. Select the country.
      1. Enter the city name, and then click ![Edit](/help/dsp/assets/search.png).
      1. Click the correct search result.
      1. Click *Include All* to include all of the locations as targets or *Exclude All* to exclude all of the locations as targets.
   * To enter or paste postal codes, and include or exclude them all:
      1. Click Paste Postal Code.
      1. Select the country.
      1. Enter or paste up to 1000 postal codes.
         Include one postal code per line, or enter multiple values separated by commas or tabs.
      1. Click *Include All* to include all of the locations as targets or *Exclude All* to exclude all of the locations as targets.
   * To remove a location from the Included or Excluded list, click **X** next to the location in the right column.
1. Click *Done*.

>[!NOTE]
>
>* Not all countries have State, City, or Postal Code locations.
>* DMA (designated market area), Federal Legislative Districts, and State Legislative Districts are available for U.S. locations only.

## Inventory Targeting

**Inventory Sources:** Inventory sources to include or exclude as targets. For most placement types, all inventory types, and all sources for each type, are included by default. For Roku placements, you must specify the inventory type and sources. You can choose from the following types of inventory:

* Public: (All placement types except for Roku) All of the open exchange inventory to which Advertising Cloud has access. You can include and exclude public inventory.

    You can view the list by source or by feed. When you view the list by feed, you can search by feed name, feed key, or a selected characteristic tag.

* Private | Roku Private: Your existing private deals (or existing private Roku deals for Roku placements) with publishers that you've set up in DSP. You can include, but not exclude, public inventory.

    You can search the list by keyword, key, deal ID, or custom tag.

* On Demand | Roku On Demand: All premium, non-guaranteed [On Demand Inventory](/help/dsp/inventory/on-demand-inventory-about.md) (or On Demand Roku deals for Roku placements) to which you've subscribed in DSP. You can include and exclude On Demand inventory.

    You can view the list by source or by feed. When you view the list by feed, you can search by feed name, feed key, or a selected publisher region, category tag, or characteristic tag.

To specify inventory targeting:

* To exclude an inventory type, clear the check box next to the name.
* To target an inventory type:
   1. Select the check box next to the inventory type name.
   1. (Optional) Change the sources to include:
      1. Click ![Edit](/help/dsp/assets/edit.png).
      1. (Public and On Demand inventory) Click **View by Source** or **View by Feed** to change how the sources are listed.
      1. (When applicable) Filter the inventory as needed.
      1. Specify the sources to include and exclude:
         * To include a Public or On Demand source, click **Include** next to the source name.
         * To include Private sources:
            * To include all inventory in a deal, click **Include all** next to the deal name.
            * To include an individual inventory source, expand the deal name, and then click the check box next to the source name.
         * To exclude a Public or On Demand source, click **Exclude** next to the source name.
   1. (Optional) To download a CSV file with the targeting information to your browser's Downloads location, click **Save & Export**.
   1. Click **Save**.

>[!TIP]
>
>If you subscribed to On Demand inventory but can't locate the publishers or deals to target, then check the status of the deals. For more information about statuses, see [About On Demand Premium Inventory](/help/dsp/inventory/on-demand-inventory-about.md).

## Site Targeting

**Traffic type:** The types of traffic to target. Options include **Websites** and **Apps**.

**Site tier:** (Available when **Paste list of targeted sites** is *Off*) The quality of the sites to target. Tiers 1-3 are all brand safe and have been vetted and approved by the DSP mapping team.

* *Tier 1:* Premium sites and applications that are nationally-recognizable.
* *Tier 2:* Targets Tier 1 as well as quality sites and applications that are less widely know than Tier 1.
* *Tier 3:* Targets Tiers 1-2 as well as legitimate and brand-safe sites and applications that cater to a niche audience. Use Tier 3 for reach or data targeting buys.
* *All Sites:* Targets Tiers 1-3 and new inventory that has not been screened or categorized, which you can use for reach.

>[!NOTE]
>
>Inventory is specific to the ad units in the placement.

>[!TIP]
>
>For performance campaigns, the best practice is to select *All Sites*.

**Site Categories:** (Optional; available when **Paste list of targeted sites** is *Off*) Site categories within the selected site tiers to either include or exclude (but not both) as targets. Choose from vertical site lists that Advertising Cloud has mapped based on site subject:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Specify the site categories to either include or exclude:
   * To include site categories:
      1. Click **Include categories**.
      1. Select the check box next to each category to target.
   * To exclude site categories:
      1. Click **Exclude categories**.
      1. Select the check box next to each category to exclude.
1. (Optional) To download a CSV file with the targeting information to your browser's Downloads location, click **Export**.
1. Click **Save**.

**Exclude Sites:** (Optional; available when **Paste list of targeted sites** is *Off*) Sites to exclude. You can either search for and select sites, or enter or paste domain names:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Specify the sites:
   * To search for a site:
      1. Click **Search**.
      1. Enter a keyword, select a site tier, and/or select a site category.
      1. In the search results, select the sites to exclude:
         * To exclude an individual site, select the check box next to it.
         * (When more than 50 results are available) To exclude the first 50 results, click **Exclude these 50**. To exclude all of the search results, click **Exclude these \<*NN*\>**.
   * To enter domain names:
      1. click **Paste**.
      1. Enter one or more domain names on separate lines.
      1. Click **Exclude All**.
1. Click **Done** when you're finished.

>[!NOTE]
>
>* Account-level and advertiser-level blocked site lists are also applied, in addition to the Advertising Cloud DSP [globally blocked site list](/help/dsp/introduction/features/brand-safety-media-quality.md), which includes sites deemed unsafe for ads.
>* Blocked sites lists always override targeted sites lists. If a placement both excludes and includes the same target for an ad, then the target is excluded.

**Language:** (Optional) A single language to target.

**Site List Preview** (Read-only) All targeted and blocked sites for the placement.

You can optionally export the list of targeted and blocked sites as a comma-separated values (CSV) file. To export the list, click **Export full site list*, and then open or save the file according to your browser's normal procedure.

**Paste list of targeted sites:** Allows you to target specific sites only. When you enable this option, the other site targeting options are disabled.

**Sites:** (Available when **Paste list of targeted sites** is *On*) Sites to target. You can either search for and select sites, or enter or paste domain names:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Specify the sites:
   * To search for a site:
      1. Click **Search**.
      1. Enter a keyword, select a site tier, and/or select a site category.
      1. In the search results, select the sites to include:
         * To exclude an individual site, select the check box next to it.
         * (When more than 50 results are available) To include the first 50 results, click **Include these 50**. To include all of the search results, click **Include these \<*NN*\>**.
   * To enter domain names:
      1. click **Paste**.
      1. Enter one or more domain names on separate lines.
      1. Click **Include All**.
1. Click **Done**.

## Audience Targeting

**Included Audiences:** Any audience targets for the placement, including [third-party segments, first-party segments, Adobe segments, custom segments, and saved audiences](/help/dsp/audiences/audience-settings.md). The total and active deduplicated audience size across all selected segments and saved audiences is also displayed. You can select an existing audience, create a new audience that you can reuse later, or select specific audience segments:

* To select an existing audience, click ![Select](/help/dsp/assets/chevron-down.png) next to Included Audiences, and then select the audience.
* To create a new audience, click ![Select](/help/dsp/assets/chevron-down.png) next to Included Audiences, and then select **+ Create Audience**. For instructions, see [Create a Reusable Audience](/help/dsp/audiences/reusable-audience-create.md), beginning with Step 3.
* To select specific audience segments, click **Select segments for this placement only**. Select the segment logic; for instructions, see Step 6 in [Create a Reusable Audience](/help/dsp/audiences/reusable-audience-create.md). When you're done, click **Save**.

**Excluded Audiences:** Any audiences to exclude for the placement, including audiences with [third-party segments, first-party segments, Adobe segments, custom segments, and saved audiences](/help/dsp/audiences/audience-settings.md). The total and active deduplicated audience size across all excluded audiences is also displayed. You can select an existing audience or create a new audience that you can reuse later:

* To select an existing audience, click ![Select](/help/dsp/assets/chevron-down.png) next to Excluded Audiences, and then select the audience.
* To create a new audience, click ![Select](/help/dsp/assets/chevron-down.png) next to Excluded Audiences, and then select **+ Create Audience**. For instructions, see [Create a Reusable Audience](/help/dsp/audiences/reusable-audience-create.md), beginning with Step 3.

**Cross Device Targeting:** (Available when you select at least one segment or audience and the [campaign is configured for people-based cross-device targeting](/help/dsp/campaign-management/campaigns/campaign-settings.md). Allows you to extend your targeting across all of a person's known devices (per the device graph specified in the campaign settings), even devices that aren't in the specified segments. Fees may apply depending on the graph specified for the campaign. Device graph data is currently only available in North America.

**Placement Cap:** (Optional) The number of times a unique device or person (depending on the specified Cross Device Level) will be served ads from the placement. Options include *Unlimited* or a specific amount per day, week, or month.

>[!NOTE]
>
> You can set frequency caps at the campaign, package, and placement levels. DSP will respect the strictest frequency cap in the campaign hierarchy.

**Secondary Cap:** (Optional; available when you include a numeric Placement Cap) An additional limitation within the bounds of the primary placement cap. Select the number of impressions and the time period (such as 3 per 12 hours).

**Day Parting:** (Optional) Specific days of the week and time of day in which ads may run. To specify dayparting intervals:
1. Click ![Edit](/help/dsp/assets/edit.png).
1. Select the applicable time zone.
1. Specify the intervals:
   * To select a preset interval, click one of the interval buttons. Options include *Weekends**, **Weekdays**, **Morning**, **Lunch**, **Dinner**, or **Prime** (primetime).
   * To manually select an interval, click inside a cell and optionally drag to select the interval.
1. Click **Save**.
 
**Topic Targeting:** (Optional; available to advertisers configured with Comscore and Grapeshot segments) Specific site topics (keywords) from Comscore and Grapeshot to include and exclude as targets. Additional fees may apply for this feature. To activate this feature and set up topic segments, contact your Adobe account manager.

To specify topic targeting:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Specify the topics to target and exclude:
   1. In the left column, select the partner (*Comscore* or *Grapeshot*).
   1. In the input field, enter the segment names or segment IDs.
1. (Optional) To download a CSV file with the topic information to your browser's Downloads location, click **Export**.
1. Click **Save**.

>[!TIP]
>
>Topic targeting limits the inventory on which the placement can bid, so use topic targeting for only a small percentage of your overall buy.

**Device Targeting:** (Optional) Specific device information, including device types, manufacturers, operating systems, browsers, and connectivity types, to include and exclude as targets. To specify device targeting:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Specify the device details to include and exclude:
   1. In the left column, select the category.
   1. Specify targeting:
      * To include a value, click **Include** next to the value name.
      * To exclude a value, click **Exclude** next to the value name.
1. (Optional) To download a CSV file with the device targeting information to your browser's Downloads location, click **Export**.
1. Click **Save**.

**ISP Targeting:** (Optional) Specific internet service providers (ISPs) to either include or exclude (but not both) as targets. To specify ISP targeting:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Specify the ISPs to include or exclude:
   * To include ISPs:
      1. Click **Include ISPs**.
      1. (Optional) Filter the list by keyword.
      1. Select the check box next to each ISP to target.
   * To exclude ISPs:
      1. Click **Exclude ISPs**.
      1. (Optional) Filter the list by keyword.
      1. Select the check box next to each ISP to exclude.
1. (Optional) To download a CSV file with the ISP targeting information to your browser's Downloads location, click **Export**.
1. Click **Save**.

## Brand Safety and Media Targeting

**Contextual filtering:** Types of Comscore, DoubleVerify, Integral Ad Science, and Peer39 contextual filters to apply. The advertiser-level defaults are selected for new placements, but you can change the settings:

* DoubleVerify:

   * **Block sites that are:** (Optional) One or more types of inventory context to block by default. Additional fees may apply.

* Peer 39:

   * **Target sites that are:** (Optional) One or more types of inventory attributes to target by default. Additional fees may apply.

* ComScore:

   * **Block sites that are:** (Optional) One or more types of inventory attributes to block by default. Additional fees may apply.

* Integral Ad Science

   * **Adult Content:** (Optional) The degree of adult content for which to block ads by default: *Do Not Block* (the default), *Standard*, or *Strict*. Additional fees may apply.

   * **Alcohol Content:** (Optional) The degree of alcohol content for which to block ads by default: *Do Not Block* (the default), *Standard*, or *Strict*. Additional fees may apply.

**Pre-bid fraud blocking:** Types of sites to block based on fraudulent traffic and suspicious activities measured through DoubleVerify, Integral Ad Science, and Peer39. The advertiser-level defaults are selected for new placements, but you can change the settings:

* DoubleVerify:

   * **Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices:** By default, blocks all 100% invalid traffic, including traffic on highjacked devices, for new placements. Additional fees may apply.
   
   * **Also block sites with:** (Optional) An additional level of fraud and invalid traffic that will cause DSP to block ads by default:  *None* (the default, which doesn't block additional traffic), *>2% Average Fraud/IVT levels (lowest reach)*, *>4% Average Fraud/IVT levels*, *>6% Average Fraud/IVT levels*, *>10% Average Fraud/IVT levels*, or *>25% Average Fraud/IVT levels*. Additional fees may apply.

* Peer 39:

   * **Block sites that are:** (Optional) One or more types of fraud that will cause DSP to block ads by default: *Fraud* (which blocks all sites with fraud), *Fraud: Bot Sites_Non-Human traffic*, and/or *Fraud: Zero Ads*. Additional fees may apply.

* Integral Ad Science:

   * **Block sites that are:** (Optional) A type of suspicious website or app activity that will cause DSP to block ads by default: *None* (the default, which doesn't block ads based on suspicious activity), *Suspicious Activity - High Risk*, or *Suspicious Activity - High or Moderate Risk*. Additional fees may apply.

**Ads.txt filtering:**

Which level of [Ads.txt](https://iabtechlab.com/ads-txt-about/) pre-bid filtering to use by leveraging each publisher's Authorized Digital Sellers list. The advertiser-level default is selected for new placements, but you can change the settings:

* *Opt out of ads.txt (default)*: To buy inventory from all sellers.
* *Ads.txt sellers + sites without ads.txt*: To prioritize buying inventory from a domain's authorized direct sellers and resellers.
* *Ads.txt sellers only*: To buy inventory only from a domain's authorized direct sellers and resellers.
* *Ads.txt sellers only*: To buy inventory only from a domain's authorized direct sellers.

**DoubleVerify Authentic Brand Safety:** (Advertisers configured with the DoubleVerify Authentic Brand Safety option) Enables DoubleVerify Authentic Brand Safety, which blocks impressions post-bid using the custom brand safety rules configured for the specified segment ID. DSP bills your account for usage for the segment ID specified in the advertiser settings.

## Tracking

>[!NOTE]
>
>(Roku placements) Third-party tracking vendors approved by Roku include Acxiom, comScore, Data Plus Math, Experian, Factual, Kantar, Marketing Evolution, Neustar, Nielsen, Nielsen Catalina Solutions, NinthDecimal, Oracle, Placed, Polk, and Research Now.

**Event Pixels:** (Optional) Third-party event tracking pixels that will be attached by default to all new ads in the placement. To specify event pixels:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Do any of the following:
   * To select an existing pixel, select the check box in the pixel row.
   * To create a new pixel:
      1. Click **Create**.
      1. Enter the following information:
         * **Pixel name:** The pixel name; the maximum length is 500 characters. Use a name that will help you easily identify the pixel.
         * **Pixel event fires on:** The event that triggers the pixel to fire. The available events vary by ad type.
         * **Pixel type:** Whether the pixel is an *IMG URL* (1x1 pixel image file), *HTML*, or *JavaScript URL*.
         * **Pixel URL:** The URL of the pixel image.
      1. Click **Create and attach**.
   1. Click **Save**.

**Conversion Pixels:** (Optional) Conversion tracking pixels that will be attached by default to all new ads in the placement. To specify conversion pixels:

1. Click ![Edit](/help/dsp/assets/edit.png).
1. Do any of the following:
   * To select an existing pixel, select the check box in the pixel row.
   * To create a new pixel:
      1. Click **Create**.
      1. Enter the following information:
         * **Conversion pixel name:** The pixel name; the maximum length is 500 characters. Use a name that will help you easily identify the pixel.
         * **Conversion category:** The type of conversion.
         * **Impression conversion window:** The number of days after an ad impression occurs in which the impression can be attributed to a conversion. The default is 30 days.
         * **Click conversion window:** The number of days after an ad click occurs in which the click can be attributed to a conversion. The default is 30 days.
         * **Notes:** (Optional) A description or other information about the pixel.
      1. Click **Create and attach**.
      1. Implement the conversion pixel on the relevant webpages:
         1. In the main menu, go to **Resources > Conversion pixels**.
         1. In the pixel row, click **edit**.
         1. Copy the value(s) in the HTLM Tag and/or Flash Tag fields, as needed, to provide to the advertiser or website contact.

            The advertiser's IT department or other group may need to schedule, or be informed about, the tag deployment.
   1. Click **Save**.

**3rd-party Fees:** (Optional) Any static third-party fee to be tracked as non-billable costs. The package-level default is automatically applied for new placements, when applicable, unless you enter a different value as the cost per thousand impressions.

>[!NOTE]
>
>Billable fees are reflected in the Net CPM metric.

>[!MORELIKETHIS]
>
>* [About Placement Management](placement-about.md)
>* [Create a Placement](placement-create.md)
<!-- >* [Edit a Placement](placement-edit.md) -->
>* [Keyboard Shortcuts](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* [FAQs About Campaign Management](/help/dsp/campaign-management/campaign-management-faq.md)
