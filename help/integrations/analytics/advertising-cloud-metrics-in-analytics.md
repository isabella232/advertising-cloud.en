---
title: Advertising Cloud Metrics in Analysis Workspace
description: Advertising Cloud Metrics in Analysis Workspace
feature: integration with Adobe Analytics
exl-id: d740bd19-c643-4917-9cfd-f9cf0affd07e
---
# Advertising Cloud Metrics in Analysis Workspace

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

>[!NOTE]
>
>* Advertising Cloud passes traffic metrics and dimensions to Analytics daily.
>* Analytics captures Advertising Cloud click-throughs and view-throughs in real time.

## Traffic Metrics from Advertising Cloud

>[!NOTE]
>
>All Advertising Cloud traffic metrics in Analytics start with "AMO".

| Traffic Metric | Description |
| -------------- | ----------- |
| AMO Impressions | The number of Advertising Cloud impressions. |
| AMO Clicks | The number of total Advertising Cloud clicks. |
| AMO Cost | The Advertising Cloud spend in the currency of the report suite. |
| AMO ID Instance | The number of times the Advertising Cloud ID is set. |
| AMO Minutes Viewed | The number of minutes an Advertising Cloud video was viewed. |
| AMO Views | The number of views on an ad. A view is counted when the viewer initiates the Advertising Cloud video. |
| AMO Views 25% Complete | The number of views for which at least 25% of an Advertising Cloud video was watched. |
| AMO Views 50% Complete | The number of views for which at least 50% of an Advertising Cloud video was watched. |
| AMO Views 75% Complete | The number of views for which at least 75% of an Advertising Cloud video was watched. |
| AMO Views 100% Complete | The number of views for which 100% of an Advertising Cloud video was watched. |
| AMO Viewable Impressions | The number of impressions that were measured to be viewable according to the placement configuration. |
| AMO Not Viewable Impressions | The number of impressions that were determined to be not viewable. Not Viewable Impressions is calculated as (Measurable Impressions - Viewable Impressions). |
| AMO Measurable Impressions | The number of impressions that were served for which viewability instrumentation successfully initialized. Measurable Impressions is calculated as (Instrumented Impressions - the number of unmeasurable impressions). |

<!--
* AMO Impressions: The total number of Advertising Cloud impressions.
* AMO Clicks: The total number of total Advertising Cloud clicks.
* AMO Cost: The total Advertising Cloud spend in the currency of the report suite.
* AMO ID Instance: The total number of times the Advertising Cloud ID is set.
* AMO Minutes Viewed: The total number of minutes an Advertising Cloud video was viewed.
* AMO Views: The total number of views on an ad. A view is counted when the viewer initiates the Advertising Cloud video.
* AMO Views 25% Complete: The number of views for which at least 25% of an Advertising Cloud video was watched.
* AMO Views 50% Complete: The number of views for which at least 50% of an Advertising Cloud video was watched.
* AMO Views 75% Complete: The number of views for which at least 75% of an Advertising Cloud video was watched.
* AMO Views 100% Complete: The number of views for which 100% of an Advertising Cloud video was watched.
* AMO Viewable Impressions: The number of impressions that were measured to be viewable according to the placement configuration.
* AMO Not Viewable Impressions: The number of impressions that were determined to be not viewable. Not Viewable Impressions is calculated as (Measurable Impressions - Viewable Impressions).
* AMO Measurable Impressions: The number of impressions that were served for which viewability instrumentation successfully initialized. Measurable Impressions is calculated as Instrumented Impressions minus the number of unmeasurable impressions.
-->

## Useful Custom Calculated Metrics for Advertising Cloud

Consider creating the following metrics for your Advertising Cloud data.

* Clicks to Landing Page Instance (AMO ID Instances / AMO Clicks): This is the % of people who clicked the ad and made it to the landing page.
* Measurable Rate (AMO Viewable Impressions / AMO Impressions * 100)
* Viewable Impression Rate (AMO Viewable Impressions / AMO Measureable Impressions * 100)
* Cost Per View (AMO Cost / AMO Views)
* Cost Per Click (AMO Cost / AMO Clicks)

## Advertising Cloud Dimensions

>[!NOTE]
>
>All Advertising Cloud dimensions in Analytics are followed by "(AMO ID)."

| Dimension | Applicable Advertising Cloud Data  | Description |
| ----------- | ---------- | ---------- |
| Ad Platform (AMO ID) | DSP and Search data | Advertising Cloud DSP or the search engine name |
| Account (AMO ID) | DSP and Search data | The account name. |
| Network (AMO ID) | DSP and Search data | RTB (DSP) or the ad network name (Search) |
| Campaign (AMO ID) | DSP and Search data | The campaign name. |
| Optimization (AMO ID) | DSP and Search data | The package (DSP) or portfolio (Search) name. |
| Placement (AMO ID) | DSP data | The placement name. |
| Ad Group (AMO ID) | Search data | The ad group name. |
| Keyword (AMO ID) | Search data | The keyword. |
| Match Type (AMO ID) | Search data | The search match type. |
| Keyword Match Type (AMO ID) | Search data | The keyword and match type. |
| Ad Type (AMO ID) | DSP and Search data | The ad type, such as *text*, *video*, *display*, or *native*. |
| Ad Title (AMO ID) | DSP and Search data |The ad type (DSP) or ad title (Search). |
| Ad Description (AMO ID) | DSP and Search data | The ad description (DSP) or ad body (Search). |
| Ad Display URL (AMO ID) | Search data | The URL displayed in the ad. |
| Ad Destination URL (AMO ID) | Search data | The destination URL for the ad. |
| Landing Type (AMO ID) | DSP and Search data | Whether the landing page entry was a view-through or a click-through. |
| Product Target (AMO ID) | Search data | The product target for a product listing ad. |

>[!MORELIKETHIS]
>
>* [Overview of Analytics for Advertising Cloud](overview.md)
>* [Analytics Data in Advertising Cloud](/help/integrations/analytics/analytics-data-in-advertising-cloud.md)
