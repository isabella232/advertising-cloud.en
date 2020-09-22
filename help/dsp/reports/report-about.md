---
title: About Custom Reports
description: About Custom Reports
---

# About Custom Reports

Custom reports (formerly called email reports) allow you to customize the content and delivery of your report data using the campaign dimensions (such as the advertiser, placement, sites, or geos) and the metrics that matter most to you. You can either:

* Completely configure campaign performance reports at a granular level.
* Choose from pre-configured report templates, and optionally customize them further.

You can generate reports once, or schedule them to be generated daily, weekly, or monthly at 03:00 in the specified time zone. Once a report is generated, a notification is sent to each specified email recipient, with a link from which to download the file.

>[!NOTE]
>
>You can also view on-demand data at all levels of a campaign (campaign, package, placement, ad, or survey) [within the relevant campaign management view](/help/dsp/campaign-management/reports/campaign-reports-about.md).

## Available Report Types

* Custom
* Pre-configured Report Templates
    * **Custom:** This is a blank template you can use to create your own custom report using most dimensions and metrics. Conversion, Device, Geo, and Site reports are variations of this template with pre-selected columns and dimensions for their respective use cases.
    
    * **Billing:** Use this report to understand key billing metrics like spend metrics for media billing by campaign.
    
       >[!NOTE]
       >
       >* This report includes data about the billing segment. If a user or device is served an impression that belongs to multiple segments, only one billable segment is credited with the impression.

    * **Conversion:** Use this report to understand how your campaigns are performing based on conversion metrics captured using Advertising Cloud conversion tracking. This includes multi-touch attribution.

    * **Device:** Use this pre-populated template to see key metrics by device-related dimensions.

    * **Frequency (by Impression):** Use this report to understand the distribution of impressions shown to unique viewers (for example, how many unique viewers saw one impression, two impressions, three impressions, and so on. Data is available by placement or campaign.
           
       >[!NOTE]
       >
       >* Data is available after March 1, 2019.
       >* Frequency is estimated based on a sampling of data.
       >* For some inventory, publishers don't pass along a device identifier, which prevents frequency tracking. This report includes only impressions for which a device identifier was available.
      

    * **Frequency (by App/Site):** Use this report to understand how many unique users were reached by app or by site. You can also see how many unique users were reached via only a particular app or site ("distinct unique users").

       >[!NOTE]
       >
       >* Data is available after November 15, 2018.
       >* For some private inventory, publishers don't pass along a device identifier, which prevents frequency tracking.

    * **Geo**: Use this pre-populated template to see key metrics by geographic dimensions.

    * **Margin:** Use this report to see key metrics like margin, profit, and other spend metrics by campaign or placement.

    * **Segment:** Use this pre-populated template to see key metrics by segment.

       >[!NOTE]
       >
       >* This report is intended to show how different targeted segments perform. It uses segment membership data. When an impression is served to a person or device belonging to two or more targeted segments, this report will include one row for each segment. For this reason, totals in this report may not match actual delivery.
       >* Conversion metrics and custom goal data for segments is available after August 2, 2019. All other data for segments is available beginning after June 1, 2018.
     
    * **Site:** By default, includes standard metrics, total media net spend, and total billable net spend by site.

>[!MORELIKETHIS]
>
>* [Create a Custom Report](/help/dsp/reports/report-create.md)
>* [Custom Report Settings](/help/dsp/reports/report-settings.md)
>* [About In-Platform Reports](/help/dsp/campaign-management/reports/campaign-reports-about.md)
<!-- >* [Available Report Metrics](/help/dsp/reports/report-metrics.md) -->
