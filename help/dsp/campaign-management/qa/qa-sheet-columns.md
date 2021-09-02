---
title: Columns in Downloaded/Uploaded Spreadsheets
description: Reference the columns in downloaded and uploaded Excel QA spreadsheets.
feature: Placements
---

# Columns in Downloaded/Uploaded Spreadsheets

<!-- rename -- not specific enough - I think you can download Excel files of other things too -->

<!-- see notes within the table about descriptions that need to be edited -->

>[!TIP]
>
> In a downloaded spreadsheet, all editable columns are highlighted in blue.

<!-- I'm not sure why options below are formatted with HTML "i" and "b" tags -- won't asterisks (Markdown) work? -->

| Section | Column | Description | Editable? |
|---------|--------|-------------|-----------|
| [!UICONTROL Basic] | [!UICONTROL Placement ID] | The numeric ID of the placement. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Placement Name] | The name of the placement. | Yes |
| [!UICONTROL Basic] | [!UICONTROL Labels] | Any applied labels, for reporting. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Edit Link] | A link to open the placement in Edit mode. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Status] | The placement status: *[!UICONTROL active]* or *[!UICONTROL inactive]*. | Yes |
| [!UICONTROL Basic] | [!UICONTROL Placement Type] | The placement type. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Package Name] | The name of the parent package, when applicable. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Start Date] | The start date of the placement. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL End Date] | The end date of the placement. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL] Day parting | Whether dayparting is <i>[!UICONTROL ON]</i> or <i>[!UICONTROL OFF]</i>.<br><b>Note:</b> To check the actual dayparting schedule, open the placement settings in [!DNL DSP]. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Budget] | The placement budget, if there is one. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Budget Interval] | The budget interval: <i[!UICONTROL >Daily]</i>, <i>[!UICONTROL Weekly]</i>, <i>[!UICONTROL Monthly]</i>, or <i>[!UICONTROL All Time]</i>. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Optimization Goal] | The objective of the package. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Optimization Target] | The target value of the goal. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Pace on] | Whether the placement is pacing towards the <i>[!UICONTROL Budget]</i> or <i>[!UICONTROL Impressions]</i>. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Max Bid] | The maximum bid for the placement. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Pacing Fill Strategy] | The pacing fill strategy for the placement: <i>[!UICONTROL evenly]</i>, <i>[!UICONTROL frontload]</i>, or <i>[!UICONTROL aggressive frontload]</i>. | Yes |
| [!UICONTROL Goals] |[!UICONTROL  Pre-Bid Filters] | Any pre-bid filter criteria to be applied. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Bidding Rules] | Whether bidding rules (deprecated) are <i>[!UICONTROL ON]</i> or <i>[!UICONTROL OFF]</i>. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap] | The primary frequency cap for the placement during the specified [!UICONTROL Frequency Cap Interval]. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap Interval] | The interval for the primary frequency cap: <i>[!UICONTROL Day]</i>, <i>[!UICONTROL Week]</i>, or <i>[!UICONTROL Month]</i>. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap] | The secondary frequency cap for the placement during the specified [!UICONTROL Secondary Frequency Cap Interval] | Yes |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval] | The type of interval for the secondary frequency cap: <i>[!UICONTROL Week]</i>, <i>[!UICONTROL Day]</i>, <i>[!UICONTROL Hour]</i>, or <i>[!UICONTROL Minute]</i>. The applicable number of weeks, days, hours, or minutes is indicated by the [!UICONTROL Secondary Frequency Cap Interval Value]. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval Value] | The number of weeks, days, hours, or minutes for which the [!UICONTROL Secondary Frequency Cap] applies. For example, if the secondary cap is three impressions per six hours, then the value here would be <b>6</>.  | Yes |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included #] | The number of targeted geographical locations, <i>[!UICONTROL All]</i>, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included] | The targeted geographical locations, separated by semi-colons,or <i>[!UICONTROL All Locations]</i>. | &mdash; |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded #] | The number of excluded geographical locations or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded] | The excluded geographical locations, separated by semi-colons,  or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Included #] | The number of targeted public inventory deals, if any are specified, <i>[!UICONTROL All]</i>, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Excluded #] | The number of excluded public inventory deals, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Included #] | The number of targeted private inventory deals, if any are specified, <i>[!UICONTROL All]</i>, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Excluded #] | The number of excluded private inventory deals, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Included #] | The number of targeted [!UICONTROL On-Demand Inventory] deals, if any are specified, <i>[!UICONTROL All]</i>, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Excluded #] | The number of excluded On-Demand Inventory deals, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Traffic Type] | The targeted type of traffic: <i>[!UICONTROL Website]</i> and/or <i>[!UICONTROL Apps]</i> | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Exclude out-stream] | Whether the Inventory Targeting option to exclude outstream traffic is <i[!UICONTROL >ON]</i> or <i>[!UICONTROL OFF]</i>.<br>Outstream ads usually appear over the content as a pop-up or stuffed into content (in the native experience), rather than as regular video ads in a video player. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Site Tier] | The quality of the sites to target: <i>[!UICONTROL Tier 1]</i>, <i>[!UICONTROL Tier 2]</i>, <i>[!UICONTROL Tier 3]</i>, or <i>[!UICONTROL All Sites]</i>. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Categories - Included #] | The number of targeted site categories, if any are specified, or <i>[!UICONTROL All]</i>. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Categories - Excluded #] | The number of excluded site categories, if any are specified, or <i>[!UICONTROL All]</i>. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Excluded Sites] | The excluded sites, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Language] | The targeted site languages. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Allow unscreened sites] | Whether or not to allow ad delivery on non-audited sites: <i>[!UICONTROL ON]</i> or <i>[!UICONTROL OFF]</i>. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Targeted Sites] | The number of targeted sites, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Included] | The targeted audiences, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Excluded] | The excluded audiences, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Demographic booster] | Whether or not [!DNL Comscore] demographic segments are enabled for the placement (and other placements in the campaign): <i>[!UICONTROL ON]</i> or <i>[!UICONTROL OFF]</i>. This feature may be enabled only for campaigns for which the [!DNL Audience Verification] feature is enabled for [!DNL Nielson] and/or [!DNL Comscore].  It incurs additional fees.  | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Extend across screens] | Whether or not to extend the ad targeting across devices: <i>[!UICONTROL ON]</i> or <i>[!UICONTROL OFF]</i>.<!-- Whether or not the Cross Device Targeting setting is enabled for the placement : <i>ON</i> or <i>OFF</i>. Cross-device targeting extends your targeting across all of a person's known device, per the device graph specified in the campaign settings.--> | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting] - Included # | The number of targeted topic codes, if any are specified, or <i>[!UICONTROL All]</i>.   | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting - Excluded #] | The number of excluded topic codes, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Included #] | The number of targeted device targets, if any are specified, or <i>[!UICONTROL All]</i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Excluded #] | The number of excluded device targets, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Included #] | The number of targeted ISP providers, if any are specified, or <i>[!UICONTROL All]/i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Excluded #] | The number of excluded ISP providers, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Contextual Filtering #] | The number of brand safety filters applied, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Fraud blocking #] | The number of pre-bid fraud blocking filters applied, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Viewability #] | The number of pre-bid viewability filters applied, if any are specified, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Site Safety Block] | Whether or not Site Safety Block is enabled: <i>[!UICONTROL ON]</i> or <i>[!UICONTROL OFF]</i>.<!-- Whether or not the advertiser-level setting Enable Site Safety Block is enabled: <i>ON</i> or <i>OFF</i>.I don’t see this option at the placement level. Should there be one? --> | &mdash; |
| [!UICONTROL Tracking] | [!UICONTROL Tracking Pixels #] | The number of third-party  event-tracking pixels attached to the placement, or <i>[!UICONTROL None]</i>.| &mdash; |
| [!UICONTROL Tracking] | [!UICONTROL Conversion Pixels #] | The number of conversion tracking pixels attached to the placement, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Tracking] | [!UICONTROL 3rd-party fees] | A static, third-party fee rate to be tracked as a non-billable cost per thousand impressions, if applicable. | &mdash; |
| [!UICONTROL Ads] | [!UICONTROL # of Ads Attached] | The number of ads attached to the placement, if any are attached, or <i>[!UICONTROL None]</i>. | &mdash; |
| [!UICONTROL Ads] | [!UICONTROL Ad Names] | The names of the ads attached to the placement, if any are attached, or <i>[!UICONTROL None]</i>. | &mdash; |

{style="table-layout:auto"}

>[!MORELIKETHIS]
>
>* [About Correcting Placement Settings for a Campaign Using Spreadsheets](qa-about.md)
>* [Download Placement Settings for a Campaign](qa-sheet-download.md)
>* [Upload Placement Settings for a Campaign](qa-sheet-upload.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
