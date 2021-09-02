---
title: Advertising Cloud Metrics in Analysis Workspace
description: Advertising Cloud Metrics in Analysis Workspace
feature: Integration with Adobe Analytics
exl-id: d740bd19-c643-4917-9cfd-f9cf0affd07e
---
# Advertising Cloud Metrics in Analysis Workspace

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

>[!NOTE]
>
>* Advertising Cloud passes traffic metrics and dimensions to [!DNL Analytics] daily.
>* [!DNL Analytics] captures Advertising Cloud click-throughs and view-throughs in real time.

## Traffic Metrics from Advertising Cloud

>[!NOTE]
>
>All Advertising Cloud traffic metrics in [!DNL Analytics] start with "AMO."

| Traffic Metric | Description |
| -------------- | ----------- |
| [!UICONTROL AMO Impressions] | The number of Advertising Cloud impressions. |
| [!UICONTROL AMO Clicks] | The number of total Advertising Cloud clicks. |
| [!UICONTROL AMO Cost] | The Advertising Cloud spend in the currency of the report suite. |
| [!UICONTROL AMO ID Instance] | The number of times the Advertising Cloud ID is set. |
| [!UICONTROL AMO Minutes Viewed] | The number of minutes an Advertising Cloud video was viewed. |
| [!UICONTROL AMO Views] | The number of views on an ad. A view is counted when the viewer initiates the Advertising Cloud video. |
| [!UICONTROL AMO Views 25% Complete] | The number of views for which at least 25% of an Advertising Cloud video was watched. |
| [!UICONTROL AMO Views 50% Complete] | The number of views for which at least 50% of an Advertising Cloud video was watched. |
| [!UICONTROL AMO Views 75% Complete] | The number of views for which at least 75% of an Advertising Cloud video was watched. |
| [!UICONTROL AMO Views 100% Complete] | The number of views for which 100% of an Advertising Cloud video was watched. |
| [!UICONTROL AMO Viewable Impressions] | The number of impressions that were measured to be viewable according to the placement configuration. |
| [!UICONTROL AMO Not Viewable Impressions] | The number of impressions that were determined to be not viewable. This value is calculated as ([!UICONTROL AMO Measurable Impressions] - [!UICONTROL AMO Viewable ]). |
| [!UICONTROL AMO Measurable Impressions] | The number of impressions that were served for which viewability instrumentation successfully initialized. This value is calculated as (instrumented impressions - the number of unmeasurable impressions). |

## Useful Custom Calculated Metrics for Advertising Cloud

Consider creating the following metrics for your Advertising Cloud data.

* Clicks to Landing Page Instance ([!UICONTROL AMO ID Instances] / [!UICONTROL AMO Clicks]): This is the % of people who clicked the ad and made it to the landing page.
* Measurable Rate ([!UICONTROL AMO Viewable Impressions] / [!UICONTROL AMO Impressions] * 100)
* Viewable Impression Rate ([!UICONTROL AMO Viewable Impressions] / [!UICONTROL AMO Measureable Impressions] * 100)
* Cost Per View ([!UICONTROL AMO Cost] / [!UICONTROL AMO Views])
* Cost Per Click ([!UICONTROL AMO Cost] / [!UICONTROL AMO Clicks])

## Advertising Cloud Dimensions

>[!NOTE]
>
>All Advertising Cloud dimensions in [!DNL Analytics] are followed by "(AMO ID)."

| Dimension | Applicable Advertising Cloud Data  | Description |
| ----------- | ---------- | ---------- |
| [!UICONTROL Ad Platform (AMO ID)] | [!DNL DSP] and [!DNL Search] data | Advertising Cloud DSP or the search engine name |
| [!UICONTROL Account (AMO ID] | [!DNL DSP] and [!DNL Search] data | The account name. |
| [!UICONTROL Network (AMO ID)] | [!DNL DSP] and [!DNL Search] data | RTB ([!DNL DSP]) or the ad network name ([!DNL Search]) |
| [!UICONTROL Campaign (AMO ID)] | [!DNL DSP] and [!DNL Search] data | The campaign name. |
| [!UICONTROL Optimization (AMO ID)] | [!DNL DSP] and [!DNL Search] data | The package ([!DNL DSP]) or portfolio ([!DNL Search]) name. |
| [!UICONTROL Placement (AMO ID)] | [!DNL DSP] data | The placement name. |
| [!UICONTROL Ad Group (AMO ID)] | [!DNL Search] data | The ad group name. |
| [!UICONTROL Keyword (AMO ID)] | [!DNL Search] data | The keyword. |
| [!UICONTROL Match Type (AMO ID)] | [!DNL Search] data | The search match type. |
| [!UICONTROL Keyword Match Type (AMO ID)] | [!DNL Search] data | The keyword and match type. |
| [!UICONTROL Ad Type (AMO ID)] | [!DNL DSP] and [!DNL Search] data | The ad type, such as `text`, `video`, `display`, or `native`. |
| [!UICONTROL Ad Title (AMO ID)] | [!DNL DSP] and [!DNL Search] data |The ad type ([!DNL DSP]) or ad title ([!DNL Search]). |
| [!UICONTROL Ad Description (AMO ID)] | [!DNL DSP] and [!DNL Search] data | The ad description ([!DNL DSP]) or ad body ([!DNL Search]). |
| [!UICONTROL Ad Display URL (AMO ID)] | [!DNL Search] data | The URL displayed in the ad. |
| [!UICONTROL Ad Destination URL (AMO ID)] | [!DNL Search] data | The destination URL for the ad. |
| [!UICONTROL Landing Type (AMO ID)] | [!DNL DSP] and [!DNL Search] data | Whether the landing page entry was a view-through or a click-through. |
| [!UICONTROL Product Target (AMO ID)] | [!DNL Search] data | The product target for a product listing ad. |

>[!MORELIKETHIS]
>
>* [Overview of [!DNL Analytics for Advertising Cloud]](overview.md)
>* [[!DNL Analytics] Data in Advertising Cloud](/help/integrations/analytics/analytics-data-in-advertising-cloud.md)
