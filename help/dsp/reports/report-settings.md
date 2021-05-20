---
title: Custom Report Settings
description: See descriptions of the custom report settings.
feature: custom reports
---

# Custom Report Settings

**Name** The report name. The maximum length is 180 characters.

**Report Type** The type of report: *Custom* (which includes most available options), *Billing*, *Conversion*, *Device*, *Frequency (by Impression)*,  *Frequency (by App/Site)*, *Geo*, *Margin*, *Media Performance*,  *Segment*, *Site*

## Apply Filters Section

**Timezone:** The timezone for reporting.

**Observe Daylight Savings Time:** Considers Daylight Saving Time in the reported times.

**\[Date Range\]:** The date range for which to generate data. The number of days available varies by report and by the selected dimensions. Choose one:

* **Previous N days:** Includes data for a specific number of days before today.

* **Custom:** Includes data between specific beginning and end dates. To report data through the previous day, select **Present**.

* **Last Calendar Month:** Includes data for the previous calendar month.

**Add Filters:** (Optional) Additional dimensions by which to filter the data, whether or not the dimensions are included as columns in the report: *Account* \*, *Advertiser*, *Campaign*, *Placement*, *Ad*, *Ad Type*, *Video*, *Video Duration*, *Country*, *Package*.

\* *Account* is available for the following report types only when your organization is configured for [cross-account reporting](report-about.md#cross-account-reporting):  Custom, Site, Segment, Geo, Device, Frequency by Impression, and Conversion. Contact your Adobe account manager for more information about cross-account reporting.

To apply one or more filters, do the following:

* Select a dimension, select the operator (*equals* or *not equals*), and then select the applicable value. For example, to return data for only preroll ads, specify "Ad Type equals Preroll."
* (Optional) Add additional criteria to the filter.
* (Optional) Add additional filters, each with one or more criteria.

## Build Your Report Section

**Select To Add As Report Headers:**  The data columns, or headers, to include in the report. To add a column, expand the category and select the check box next to the column name. All unavailable metrics are disabled. The available data categories include:

* Dimensions
* Metrics
* Conversion Metrics (sorted by advertiser)
* Custom Goals (sorted by advertiser)

**Drag to Re-Order Report Headers Below:** The order of the column headers. You can drag and drop any column to customize the order.

## Multi-Touch Conversion Options Section

**Format:** Whether to generate a report in *CSV* (comma-separated values) or *Tab* (tab-separated values) format.

**Report Headers:** Whether to *Include* or *Do Not Include* column headers.

**Attribution Rule Settings:** (All Custom, Conversion, Device, Geo, Segment, and Site reports with Conversion Metrics or Custom Goals columns; advertisers with Advertising Cloud conversion tracking only) Within the report, how to attribute conversion data in a series of events that lead to a conversion. You can choose more than one rule if you want to compare differences between the rules.

>[!NOTE]
>
>Conversion paths include any impressions and clicks within the advertiser's impression or click lookback windows, which are configured in Advertising Cloud Search. Clicks are given preference to impressions during conversion attribution. Any clicks in a conversion path receive full credit based on the attribution rule. Impressions receive credit only when no clicks are tracked in the conversion path.

* *Last Event:* Attributes conversions to the last click or impression in the conversion path.  

* *Weight Last Event More:* Attributes conversions to all events in the conversion path but gives the most weight to the last event and successively less weight to the preceding events.

* *Even Distribution:* Attributes conversions equally to each event in the conversion path.

* *Weight First Event More:* Attributes conversions to all events in the conversion path but gives the most weight to the first event and successively less weight to the following events.

* *First Event:* Attributes conversions to the first click or impression in the conversion path.

* *U-shaped:* Attributes the conversion to all events in the conversion path but gives the most weight to the first and last events, with successively less weight to the events in the middle of the conversion path.

* *Display Only - Last Event:*  Attributes conversions to the last DSP click or impression in the conversion path. This includes video and connected TV ads and excludes clicks on Search ads.

* *Social Only:* Last Event — Obsolete

<!-- See also [How Attribution Rules Are Calculated for Adobe Advertising Cloud](). -->

**Paths as Columns:**  (All Custom, Conversion, Device, Geo, Segment, and Site reports with Conversion Metrics or Custom Goals columns) Which types of conversions to report when prior events occurred on the same device. You can include up to three types. For each selected type, a separate column is included for each conversion metric and is appended with the specified suffix ((tl), (ct), or (vt)):

* *Total (TL) = CT + VT \* VT weight:* Includes conversions attributed to clicks (CT for click-through) and to impressions (VT for view-through). Conversions attributed to impressions are multiplied by the specified view-through weight. The default view-through weight is 100%, which means that conversions attributed to impressions are counted as 100% of the value of conversions attributed to clicks.

* *With Clicks (CT):* Includes only conversions attributed to clicks.

* *Impressions Only (VT):* Includes only conversions that were attributed to impressions because no clicks were tracked in the conversion path.

**Cross Device Level:**  (All Custom, Conversion, Device, Geo, Segment, and Site reports with Conversion Metrics or Custom Goals columns; applicable only for advertisers with cross-device attribution) The level at which to track conversions: *People* or *Household*.

Learn more about [cross-device solutions](/help/dsp/introduction/features/cross-device-solutions.md).

**Cross-Device Breakout:** (All Custom, Conversion, Device, Geo, Segment, and Site reports with Conversion Metrics or Custom Goals columns; applicable only for advertisers with cross-device attribution) The level of detail about cross-device conversions to include in the report. You can choose up to three levels, each of which will be included in a separate column, if you want a detailed breakout.

* *Total People (TP):* Includes the total conversions, which includes both same-device conversions and cross-device conversions (if applicable). In the report, "(tp)" is appended to the conversion metric name and rule type.

* *Same Device (SD):* Includes only conversions for which only a single device was tracked in the conversion path. In the report, "(sd)" is appended to the conversion metric name and rule type.

* *Cross Device (XD):* Includes only conversions for which more than one device was tracked in the conversion path. In the report, "(xd)" is appended to the conversion metric name and rule type.

**Conversion Reporting Based On:**  How to report conversion data:

* *Conversion Timestamp:* (The default) Conversions will be associated with the conversion date.

* *Event Timestamp:* Conversions will be reported based on the date of the impression or click that caused the conversion, as determined by the specified Attribution Rule Settings.

## Add Email Recipients Section

**Email:** Email address(es) to which to send completed reports or notifications if the report is canceled because of errors. To specify multiple addresses, separate them with commas or spaces.

**Frequency:** How often to send the report: *Once*, *Daily*, *Weekly*, or *Monthly*.

## Save Report Section

**Send & Save:** When to send the report: *On Schedule* or *Run Now*. Scheduled reports will be delivered by 09:00 in the account's timezone.

>[!NOTE]
>
>You can [run a custom report at any time](report-run-now.md) from the Reports view.

>[!MORELIKETHIS]
>
>* [About Custom Reports](/help/dsp/reports/report-about.md)
>* [Create a Custom Report](/help/dsp/reports/report-create.md)
>* [Duplicate a Custom Report](/help/dsp/reports/report-copy.md)
>* [Edit a Custom Report](/help/dsp/reports/report-edit.md)
>* [Run a Custom Report](/help/dsp/reports/report-run-now.md)
>* [Custom Report Settings](/help/dsp/reports/report-settings.md)
* [Available Report Columns](/help/dsp/reports/report-columns.md)
