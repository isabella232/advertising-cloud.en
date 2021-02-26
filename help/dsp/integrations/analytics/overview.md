---
title: Overview of Analytics for Advertising Cloud
description: Overview of Analytics for Advertising Cloud
---

# Overview of Analytics for Advertising Cloud

*Advertisers with Advertising Cloud DSP and Advertising Cloud Search*

Analytics for Advertising Cloud integrates Adobe Analytics and Adobe Advertising Cloud to extend and enhance the capabilities of each product.

The integration allows advertisers to track click-through and view-through site interactions in their Analytics instances, allowing brands to see how their advertising spend leads to site engagement and critical business objectives.

In addition, Advertising Cloud can access the vast first-party data that Analytics collects using Adobe Analytics tags already on site. This allows more robust journey management, first-party remarketing, and paid media site reporting. Advertising Cloud can further use the Adobe Analytics data for spend and bid optimization.

When properly employed, Analytics for Advertising Cloud blurs the lines between two traditional roles: advertising journey management (the act of sending users to the site through advertisements) and understanding that site engagement through web analytics.

Primary benefits:

* Send Analytics segments directly to Advertising Cloud for first-party site remarketing.
* Use Analytics custom and standard events as conversion signals for optimizing paid media advertising.
* Take advantage of Analytics Analysis Workspace to better understand site entry points and visit behavior.
* Enable closer collaboration between web analysts and paid media teams.
* Use persistent Advertising Cloud view-through and click-through IDs within Analytics to understand site engagement.
* Enhance traditional paid media reports in Analysis Workspace with custom metrics, custom dimensions, and site activity not achievable when exporting data or pixels to ad servers or other DSPs.
* Take advantage of Analytics code already on your website for tracking and optimization within Advertising Cloud.

>[!TIP]
>
> Watch a [video introduction to Analytics for Advertising Cloud](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html?lang=en#analytics).

## Using Analytics for Paid Media Reporting

Analytics for Advertising Cloud improves reporting and insight on how your advertising drives site behavior by allowing you to:

* Use persistent Advertising Cloud view-through and click-through IDs within Analytics to understand site engagement.
* Take advantage of Analysis Workspace to better understand site entry points and visit behavior. You can access paid media dimensional and event data, which include Advertising Cloud campaign entity names (down to placements and ads) and their associated metrics, such as clicks, impressions, and cost.

To use Analytics as your paid media reporting tool, your organization needs an Experience Cloud login with access to Analysis Workspace. Your Advertising Cloud team will help you to map your Advertising Cloud data to individual report suites in Analysis Workspace. You can send Advertising Cloud data to any report suite, but you should be aware of the report suites that have been mapped to Advertising Cloud and those that haven't. Depending on the report suite, this may change the data reported.

[Advertising Cloud IDs within Analytics](ids.md) works like other eVars, with a custom, persistent expiration. By default, the attribution lookback window is set to 60 days during the Advertising Cloud implementation. To change this setting, work with your Adobe account manager.

Advertising Cloud dimensions are appended with the suffix “(AMO ID)" (such as *Ad Type (AMO ID)*). See "[Advertising Cloud Metrics in Analysis Workspace](advertising-cloud-metrics-in-analytics.md)" for a list of the available dimensions.

>[!NOTE]
>
> When you view Advertising Cloud data (or any data set) within Analytics, be aware that metrics and reports are based on the rules that are set within Analytics. The data could be different than what you see within other reporting systems, such as ad server reports, DSP reports, or search engine reports. To understand the data differences in Analytics, you need to know when eVar data expires, what defines a visit, what is considered last touch attribution versus total persisting attribution, and other factors. For more information, see [Expected Data Variances Between Analytics and Advertising Cloud](data-variances.md).

## Using Analytics to Power Advertising Cloud Campaigns and Portfolios

Without requiring any additional pixels, Analytics for Advertising Cloud enables better optimization and easier audience segmentation by sending two main signals to Advertising Cloud:

* Conversion metrics to be used as bid signals:
    * standard metrics, such as Revenue and Cart Views.
    * site engagement metrics, such as page view and visit metrics.
    * custom revenue metrics.
    * reserved revenue metrics.
* Segments created in Analytics and published to Experience Cloud.
     
     You can use Analytics segments for first-party site retargeting in DSP and paid search advertisements.
     
     (Advertising Cloud Search only) Advertisers with Analytics but not Audience Manager can also create Google website tag-based audiences (remarketing lists) and customer match audiences (customer lists) from Analytics segments that are shared with Experience Cloud.

### Site Conversion Metrics as Bid Signals

You can use your standard events and custom events from Analytics to build weighted objectives in Advertising Cloud. Objectives inform bidding decisions for your DSP packages and Search portfolios.

>[!NOTE]
>
> You can't map calculated metrics from Analytics into Advertising Cloud.

Your Advertising Cloud team will help you to identify and map the events that are applicable to paid media performance into Advertising Cloud, where they will appear in [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Transaction Properties].

See "[Analytics Metrics in Advertising Cloud](analytics-metrics-in-advertising-cloud.md)" for a list of available metrics.

### Analytics Segments for Site Retargeting

Advertising Cloud can ingest Analytics segments for remarketing purposes for Advertising Cloud DSP and Search ads using the native Experience Cloud Audiences integration between Analytics and Experience Cloud.

To access the Analytics segments, an advertiser account needs to have the [Experience Cloud ID Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) enabled. When the ID Service is enabled, all Experience Cloud segments (including segments created in Analytics and published to Experience Cloud, segments created in Adobe Audience Manager, segments created in Experience Cloud using the People core service, and segments created in Adobe Experience Platform and sent to Advertising Cloud via Audience Manager) become available within Advertising Cloud as soon as they are processed.

Analytics segments take up to 24 hours to become available and are updated daily.

For more information about the Experience Cloud Audiences service, see [Experience Cloud Audiences](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html).

## Examples of How to Use the Integration

### Using Advertising Cloud Data in Analysis Workspace

 To learn how you can use your Advertising Cloud data to create visual reports in Analysis Workspace, see the video "[Introduction to Workspace and Reporting](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-analysis-workspace-a4adc.html)."

### Creating Advertising Cloud Dashboards

To learn how you can track your Advertising Cloud data against your goals in Analysis Workspace, see the video "[Create Advertising Cloud Dashboards with Adobe Analytics](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-dashboards-a4adc.html)."

### Using the Advertising Cloud ID for Site Entry Analysis

To see how you can create an Advertising Cloud site entry report to monitor day-of-week, time-of-day, browser, and geographical influences, see the video "[Create Advertising Cloud Site Entry Reports](https://experienceleague.corp.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-site-entry-a4adc.html)."

>[!MORELIKETHIS]
>
>* [Video: Introduction to Analytics for Advertising Cloud](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/intro-a4adc.html)
>* [Prerequisites and Key Information for Implementing Analytics for Advertising Cloud](prerequisites.md)
>* [Advertising Cloud IDs Used by Analytics](ids.md)
>* [JavaScript Code for Analytics for Ad Cloud](/help/dsp/integrations/analytics/javascript.md)
>* [Expected Data Variances Between Analytics and Advertising Cloud](data-variances.md)
>* [Advertising Cloud Metrics in Analysis Workspace](/help/dsp/integrations/analytics/advertising-cloud-metrics-in-analytics.md)
>* [Analytics Data in Advertising Cloud](/help/dsp/integrations/analytics/analytics-data-in-advertising-cloud.md)
