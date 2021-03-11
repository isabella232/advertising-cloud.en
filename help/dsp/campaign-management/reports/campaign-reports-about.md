---
title: About In-Platform Reports
description: About In-Platform Reports
---

# About In-Platform Reports

<!-- rename "About Performance Reports in Campaign Management Views?" -->
The campaign management views include comprehensive report data. The available reports help you to identify the packages and placements that are performing well and those that need your attention. Quick action buttons also make you more productive.

## All Campaigns List

The Campaigns view opens to a list of all campaigns within your account. The Subtotals row shows either the sum or the average value of each metric across all visible rows.

![Campaigns list](/help/dsp/assets/campaigns-list.png)

By default, each campaign row includes pacing and delivery metrics. Pacing metrics include Gross Spend (Lifetime), which includes a gauge of the actual on-target spend versus the expected on-target spend across all packages in the campaign, so you can identify under-performing campaigns at a glance. You can optionally [change the column view](column-view-change.md) or even [create a custom column view](column-view-create.md).

You can further [customize the data tables](campaign-data-views-about.md) in additional ways and [filter the visible data](campaign-data-filter.md).

To view a campaign in more detail, click the campaign name.

## Single Campaign Reporting

Within a campaign, you can filter data based on the campaign entity: Packages, Placements, and Ads. You can further [filter the visible data](campaign-data-filter.md) to include only the packages, placements, or ads that you want to see.

![Campaign entity tabs](/help/dsp/assets/campaign-subtabs.png)

In each entity tab, each row includes pacing and delivery metrics, by default, but you can [change the column view](column-view-change.md) or even [create a custom column view](column-view-create.md) to apply across all subtabs for the campaign. You can further [customize the data tables](campaign-data-views-about.md) in additional ways. Each data table includes a Subtotals row, which shows either the sum or the average value of each metric across all visible rows.

For each campaign, you can also customize time series trend charts with three metrics, which are available in each entity view. By default, data for Net Spend, Impressions, and Net CPM are included in separate charts (trellis charts). You can optionally change the metrics.

![separate trend charts for three metrics](/help/dsp/assets/trend-chart-separate.png)

You also can optionally overlay the three metrics for easy detection of anomalies and areas in which to improve scale or performance.

![trend chart with overlay](/help/dsp/assets/trend-chart.png)

You can [customize the trend charts](campaign-data-visualization-manage.md) by campaign, and the same metrics are persisted across all trend charts for the campaign.

### Placement Inspector

For each placement, you can [open a detail view (Inspector)](placement-details-view.md), which includes the following in-depth data:

* **Sites:** All of the sites on which the placement has had impressions.

   The Sites tab includes search and filter features, the same standard and custom column view options that are available on the main page, and an Exclude button in each row so you can quickly exclude a site from the placement.

* **Ads:** All of the ads in the placement.

   The Ads tab includes search and filter features, the same standard and custom column view options that are available on the main page, and quick action buttons in each row, such as Pause (so you can quickly pause an ad).

* **Frequency:** Data for each ad frequency level for the placement, including:
    * the ad frequency level (such as "1" for all instances in which users saw an ad one time)
    * the estimated unique number of devices/browsers or people (depending on the specified Cross Device Level for the placement) who received impressions at the specified frequency level
    * the estimated number of impressions at the specified frequency level
    * the estimated average frequency for the specified frequency level. This value is equal to (Estimated Impressions)/(Estimated Uniques).

![placement Inspector](/help/dsp/assets/placement-inspector-sites.png)

You can export the data on the Sites, Ads, or Frequency tab to your browser's default download folder as a report in XLSM format.

### Other Types of Campaign-level Reporting

For other data breakouts, view [the legacy campaign-level reporting pages](/help/dsp/campaign-management/campaigns/campaign-view-report.md) from Campaigns Classic. The legacy report includes sections on Geography, Device, Viewability, and Audience Performance data.

>[!MORELIKETHIS]
>
>* [View the Sites, Ads, and Frequency Details for a Placement](placement-details-view.md)
>* [About the Campaign Data Views](campaign-data-views-about.md)
>* [Create a Custom Column View](column-view-create.md)
>* [Change the Column View](column-view-change.md)
>* [Manage Data Visualizations](campaign-data-visualization-manage.md)
>* [Export Data from a Campaign Management View](campaign-export-data.md)
>* [View a Detailed Report for a Campaign](/help/dsp/campaign-management/campaigns/campaign-view-report.md)
