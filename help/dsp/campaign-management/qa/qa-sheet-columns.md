---
title: Columns in Downloaded/Uploaded Spreadsheets
description: Reference the columns in downloaded and uploaded Excel QA spreadsheets.
feature: QA sheets
---

# Columns in Downloaded/Uploaded Spreadsheets

<!-- rename -- not specific enough - I think you can download Excel files of other things too -->

<!-- see notes within the table about descriptions that need to be edited -->

>[!TIP]
>
> In a downloaded spreadsheet, all editable columns are highlighted in blue.

| Section | Column | Description | Editable? |
|--------------------|-----------------------------------------|---------------------------------------------------------------------------------|-----------|
| Basic | Placement ID | The numeric ID of the placement. | &mdash; |
| Basic | Placement Name | The name of the placement. | Yes |
| Basic | Labels | Any applied labels, for reporting. | &mdash; |
| Basic | Edit Link | A link to open the placement in Edit mode. | &mdash; |
| Basic | Status | The placement status: <i>active</i> or <i>inactive</i>. | Yes |
| Basic | Placement Type | The placement type. | &mdash; |
| Basic | Package Name | The name of the parent package, when applicable. | &mdash; |
| Goals | Start Date | The start date of the placement. | &mdash; |
| Goals | End Date | The end date of the placement. | &mdash; |
| Goals | Day parting | Whether dayparting is <i>ON</i> or <i>OFF</i>.<br><b>Note:</b> To check the actual dayparting schedule, open the placement settings in DSP. | &mdash; |
| Goals | Budget | The placement budget, if there is one | Yes |
| Goals | Budget Interval | The budget interval: <i>Daily</i>, <i>Weekly</i>, <i>Monthly</i>, or <i>All Time</i>. | Yes |
| Goals | Optimization Goal | The objective of the package. | &mdash; |
| Goals | Optimization Target | The target value of the goal. | &mdash; |
| Goals | Pace on | Whether the placement is pacing towards the <i>Budget</i> or <i>Impressions</i>. | &mdash; |
| Goals | Max Bid | The maximum bid for the placement. | Yes |
| Goals | Pacing Fill Strategy | The pacing fill strategy for the placement: <i>evenly</i>, <i>frontload</i>, or <i>aggressive frontload</i>. | Yes |
| Goals | Pre-Bid Filters | Any pre-bid filter criteria to be applied. | &mdash; |
| Goals | Bidding Rules | Whether bidding rules are <i>ON</i> or <i>OFF</i>. | &mdash; |
| Goals | Frequency Cap | The primary frequency cap for the placement during the specified Frequency Cap Interval. | Yes |
| Goals | Frequency Cap Interval | The interval for the primary frequency cap: <i>Day</i>, <i>Week</i>, or <i>Month</i>. | Yes |
| Goals | Secondary Frequency Cap | The secondary frequency cap for the placement during the specified Secondary Frequency Cap Interval | Yes |
| Goals | Secondary Frequency Cap Interval | The type of interval for the secondary frequency cap: <i>Week</i>, <i>Day</i>, <i>Hour</i>, or <i>Minute</i>. The applicable number of weeks, days, hours, or minutes is indicated by the Secondary Frequency Cap Interval Value. | Yes |
| Goals | Secondary Frequency Cap Interval Value | The number of weeks, days, hours, or minutes for which the Secondary Frequency Cap applies. For example, if the secondary cap is three impressions per six hours, then the value here would be <b>6</>.  | Yes |
| Audience Location | Audience Location - Included # | The number of targeted geographical locations, <i>All</i>, or <i>None</i>. | &mdash; |
| Audience Location | Audience Location - Included | The targeted geographical locations, separated by semi-colons (;),or <i>All Locations</i>. | &mdash; |
| Audience Location | Audience Location - Excluded # | The number of excluded geographical locations or <i>None</i>. | &mdash; |
| Audience Location | Audience Location - Excluded | The excluded geographical locations, separated by semi-colons (;),  or <i>None</i>. | &mdash; |
| Inventory | Public Inventory - Included # | The number of targeted public inventory deals, if any are specified, <i>All</i>, or <i>None</i>. | &mdash; |
| Inventory | Public Inventory - Excluded # | The number of excluded public inventory deals, if any are specified, or <i>None</i>. | &mdash; |
| Inventory | Private Inventory - Included # | The number of targeted private inventory deals, if any are specified, <i>All</i>, or <i>None</i>. | &mdash; |
| Inventory | Private Inventory - Excluded # | The number of excluded private inventory deals, if any are specified, or <i>None</i>. | &mdash; |
| Inventory | On Demand Inventory - Included # | The number of targeted On-Demand Inventory deals, if any are specified, <i>All</i>, or <i>None</i>. | &mdash; |
| Inventory | On Demand Inventory - Excluded # | The number of excluded On-Demand Inventory deals, if any are specified, or <i>None</i>. | &mdash; |
| Sites | Traffic Type | The targeted type of traffic: <i>Website</i> and/or <i>Apps</i> | &mdash; |
| Sites | Exclude out-stream | Whether the Inventory Targeting option to exclude outstream traffic is <i>ON</i> or <i>OFF</i>.<br>Outstream ads usually appear over the content as a pop-up or stuffed into content (in the native experience), rather than as regular video ads in a video player. | &mdash; |
| Sites | Site Tier | The quality of the sites to target: <i>Tier 1</i>, <i>Tier 2</i>, <i>Tier 3</i>, or <i>All Sites</i>. | &mdash; |
| Sites | Categories - Included # | The number of targeted site categories, if any are specified, or <i>All</i>. | &mdash; |
| Sites | Categories - Excluded # | The number of excluded site categories, if any are specified, or <i>All</i>. | &mdash; |
| Sites | Excluded Sites | The excluded sites, if any are specified, or <i>None</i>. | &mdash; |
| Sites | Language | The targeted site languages. | &mdash; |
| Sites | Allow unscreened sites | Whether or not to allow ad delivery on non-audited sites: <i>ON</i> or <i>OFF</i>. | &mdash; |
| Sites | Targeted Sites | The number of targeted sites, if any are specified, or <i>None</i>. | &mdash; |
| Audience Targeting | Audience - Included | The targeted audiences, if any are specified, or <i>None</i>. | &mdash; |
| Audience Targeting | Audience - Excluded | The excluded audiences, if any are specified, or <i>None</i>. | &mdash; |
| Audience Targeting | Demographic booster | Whether or not Comscore demographic segments are enabled for the placement (and other placements in the campaign): <i>ON</i> or <i>OFF</i>. This feature may be enabled only for campaigns for which the Audience Verification feature is enabled for Nielson and/or Comscore.  It incurs additional fees.  | &mdash; |
| Audience Targeting | Extend across screens | Whether or not to extend the ad targeting across devices: <i>ON</i> or <i>OFF</i>.<!-- Whether or not the Cross Device Targeting setting is enabled for the placement : <i>ON</i> or <i>OFF</i>. Cross-device targeting extends your targeting across all of a person's known device, per the device graph specified in the campaign settings.--> | &mdash; |
| Audience Targeting | Topic Targeting - Included # | The number of targeted topic codes, if any are specified, or <i>All</i>.   | &mdash; |
| Audience Targeting | Topic Targeting - Excluded # | The number of excluded topic codes, if any are specified, or <i>None</i>. | &mdash; |
| Audience Targeting | Device Targeting - Included # | The number of targeted device targets, if any are specified, or <i>All</i>. | &mdash; |
| Audience Targeting | Device Targeting - Excluded # | The number of excluded device targets, if any are specified, or <i>None</i>. | &mdash; |
| Audience Targeting | ISP Targeting - Included # | The number of targeted ISP providers, if any are specified, or <i>All</i>. | &mdash; |
| Audience Targeting | ISP Targeting - Excluded # | The number of excluded ISP providers, if any are specified, or <i>None</i>. | &mdash; |
| Brand Safety | Brand Safety - Contextual Filtering # | The number of brand safety filters applied, if any are specified, or <i>None</i>. | &mdash; |
| Brand Safety | Brand Safety - Pre-Bid Fraud blocking # | The number of pre-bid fraud blocking filters applied, if any are specified, or <i>None</i>. | &mdash; |
| Brand Safety | Brand Safety - Pre-Bid Viewability # | The number of pre-bid viewability filters applied, if any are specified, or <i>None</i>. | &mdash; |
| Brand Safety | Site Safety Block | Whether or not Site Safety Block is enabled: <i>ON</i> or <i>OFF</i>.<!-- Whether or not the advertiser-level setting Enable Site Safety Block is enabled: <i>ON</i> or <i>OFF</i>.I don’t see this option at the placement level. Should there be one? --> | &mdash; |
| Tracking | Tracking Pixels # | The number of third-party  event-tracking pixels attached to the placement, or <i>None</i>. | &mdash; |
| Tracking | Conversion Pixels # | The number of conversion tracking pixels attached to the placement, or <i>None</i>. | &mdash; |
| Tracking | 3rd-party fees | A static, third-party fee rate to be tracked as a non-billable cost per thousand impressions, if applicable. | &mdash; |
| Ads | # of Ads Attached | The number of ads attached to the placement, if any are attached, or <i>None</i>. | &mdash; |
| Ads | Ad Names | The names of the ads attached to the placement, if any are attached, or <i>None</i>. | &mdash; |

>[!MORELIKETHIS]
>
>* [About Correcting Placement Settings for a Campaign Using Spreadsheets](qa-about.md)
>* [Download Placement Settings for a Campaign](qa-sheet-download.md)
>* [Upload Placement Settings for a Campaign](qa-sheet-upload.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
