---
title: About In-Platform Reports
description: Learn about the report data included in the campaign management views.
feature: Campaign Data Views
exl-id: e9f7dafe-e0db-4fec-bf5b-858cbcfdde45
---
# About In-Platform Reports

<!-- rename "About Performance Reports in Campaign Management Views?" -->
The campaign management views include comprehensive report data. The available reports help you to identify the packages and placements that are performing well and those that need your attention. Quick action buttons also make you more productive.

## All Campaigns List

The [!UICONTROL Campaigns] view opens to a list of all campaigns within your account. The [!UICONTROL Subtotals] row shows either the sum or the average value of each metric across all visible rows.

![Campaigns list](/help/dsp/assets/campaigns-list.png)

By default, each campaign row includes pacing and delivery metrics. Pacing metrics include [!UICONTROL Gross Spend (Lifetime)], which includes a gauge of the actual on-target spend versus the expected on-target spend across all packages in the campaign, so you can identify under-performing campaigns at a glance. You can optionally [change the column view](column-view-change.md) or even [create a custom column view](column-view-create.md).

You can further [customize the data tables](campaign-data-views-about.md) in additional ways and [filter the visible data](campaign-data-filter.md).

To view a campaign in more detail, click the campaign name.

## Single Campaign Reporting

Within a campaign, you can filter data based on the campaign entity: [!UICONTROL Packages], [!UICONTROL Placements], and [!UICONTROL Ads]. You can further [filter the visible data](campaign-data-filter.md) to include only the packages, placements, or ads that you want to see.

![Campaign entity tabs](/help/dsp/assets/campaign-subtabs.png)

In each entity tab, each row includes pacing and delivery metrics, by default, but you can [change the column view](column-view-change.md) or even [create a custom column view](column-view-create.md) to apply across all subtabs for the campaign. You can further [customize the data tables](campaign-data-views-about.md) in additional ways. Each data table includes a [!UICONTROL Subtotals] row, which shows either the sum or the average value of each metric across all visible rows.

For each campaign, you can also customize time series trend charts with three metrics, which are available in each entity view. By default, data for [!UICONTROL Net Spend], [!UICONTROL Impressions], and [!UICONTROL Net CPM] are included in separate charts (trellis charts). You can optionally change the metrics.

![separate trend charts for three metrics](/help/dsp/assets/trend-chart-separate.png)

You also can optionally overlay the three metrics for easy detection of anomalies and areas in which to improve scale or performance.

![trend chart with overlay](/help/dsp/assets/trend-chart.png)

You can [customize the trend charts](campaign-data-visualization-manage.md) by campaign, and the same metrics are persisted across all trend charts for the campaign.

### Placement Inspector

For each placement, you can [open a (detail view [!UICONTROL Inspector])](placement-details-view.md), which includes the following in-depth data:

* **[!UICONTROL Sites]:** All of the sites on which the placement has had impressions.

   The [!UICONTROL Sites] tab includes search and filter features, the same standard and custom column view options that are available on the main page, and an [!UICONTROL Exclude] button in each row so you can quickly exclude a site from the placement.

* **[!UICONTROL Ads]:** All of the ads in the placement.

   The [!UICONTROL Ads] tab includes search and filter features, the same standard and custom column view options that are available on the main page, and quick action buttons in each row, such as [!UICONTROL Pause] (so you can quickly pause an ad).

* **[!UICONTROL Frequency]:** Data for each ad frequency level for the placement, including:
    * the ad frequency level (such as "1" for all instances in which users saw an ad one time)
    * the estimated unique number of devices/browsers or people (depending on the specified [!UICONTROL Cross Device Level] for the placement) who received impressions at the specified frequency level
    * the estimated number of impressions at the specified frequency level
    * the estimated average frequency for the specified frequency level. This value is equal to (Estimated Impressions)/(Estimated Uniques).

* **[!UICONTROL Inventory]:** Information for all the deals targeted by the placement in a single-view. 

The Inventory tab includes search and filter features, the same standard and custom column view options that are available on the main page, and quick action buttons in each row, such as Edit and View Report. The Inventory tab helps in quick troubleshooting by showing performance stats such as Auctions, Bids, Win Rate etc. 

# Troubleshooting Inventory

| Issue | Possible Cause  | Actions to Take |
| -----------| ---------- | ---------- |
| [!UICONTROL Zero Auctions] | Publisher has not started sending bid requests | Contact the publisher for activating the deal |
| | Deal Setup Issues like entering incorrect external deal ID etc. | Confirm the deal details and edit deal |
| [!UICONTROL Non-zero Auctions but no Bids] | The placement targeting does not match the incoming bid requests from deal. <br><br> For e.g. Placement might be targeting different geography than required as per deal | Edit placement settings suitably to avoid targeting mismatches with deal |
| | Placement does not have an active ad or correct media type as required by deal | Create/Attach ad with correct media type to the placement |
| | Placement does not have adequate budget | Edit placement budget suitably to allow bidding on incoming requests |
| | Placement flight dates do not overlap with impression delivery dates as per deal | Edit the flight dates for the placement |
| [!UICONTROL Low Win Rate] | Max bid at placement is set below the minimum required by the deal (floor or fixed) | Edit Max Bid at placement suitably |
| | The placement uses pre-bid filters that limit | Lower the thresholds of pre-bid filters to allow more bidding |
| | Audience targeting at placement is too restrictive | Check the specified audience targets have enough active users and expand audience if possible |

![placement Inspector](/help/dsp/assets/placement-inspector-sites.png)

You can export the data on the [!UICONTROL Sites], [!UICONTROL Ads], or [!UICONTROL Frequency] tab to your browser's default download folder as a report in XLSM format.

### Other Types of Campaign-level Reporting

For other data breakouts, view [the legacy campaign-level reporting pages](/help/dsp/campaign-management/campaigns/campaign-view-report.md) from [!UICONTROL Campaigns Classic]. The legacy report includes sections on [!UICONTROL Geography], [!UICONTROL Device], [!UICONTROL Viewability], and [!UICONTROL Audience Performance] data.

>[!MORELIKETHIS]
>
>* [View the Sites, Ads, and Frequency Details for a Placement](placement-details-view.md)
>* [About the Campaign Data Views](campaign-data-views-about.md)
>* [Create a Custom Column View](column-view-create.md)
>* [Change the Column View](column-view-change.md)
>* [Manage Data Visualizations](campaign-data-visualization-manage.md)
>* [Export Data from a Campaign Management View](campaign-export-data.md)
>* [View a Detailed Report for a Campaign](/help/dsp/campaign-management/campaigns/campaign-view-report.md)
