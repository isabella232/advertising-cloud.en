---
type: Documentation
cloud: Experience Cloud
solution: Advertising Cloud
product: advertising cloud
title: Analytics Data in Advertising Cloud
description: Analytics Data in Advertising Cloud
exl-id: 79fbc809-9965-41c1-971f-3652cc78fee3
---
# Analytics Data in Advertising Cloud

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

## Analytics Segments

All segments created in Analytics and published to Experience Cloud.

New segments take 24-48 hours to appear in Advertising Cloud. Updates to existing segments are synchronized within about eight hours.

## Site Engagement Metrics

>[!NOTE]
>
>* Analytics passes events for the EF ID eVar into Advertising Cloud.  The default integration doesn't support sending calculated metrics or other dimensions (eVars) into Advertising Cloud. If the calculated metric can be wholly captured in a custom event, however,then Advertising Cloud can ingest the custom event.
>* Analytics passes data to Advertising Cloud hourly.

* Timespent_secs_1stvisit: The number of seconds spent on the site during the visitor's first visit.
* Timespent_secs_total: The total number of seconds spent on the site across all visits within the click lookback window.
* Pageviews_1stvisit: The number of page views on the site during the visitor's first visit.
* Pageviews_total: The total number of page views on the site across all visits within the click lookback window.
* [Bounces](https://experienceleague.adobe.com/docs/analytics/components/metrics/bounces.html?lang=en#metrics)
* [Visits](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html?lang=en#metrics)
* ef_id_instances: The number of times that Analytics collected an EF ID.

## Conversion Metrics

Analytics passes conversion metrics to Advertising Cloud daily.

### Standard Conversion Metrics

* [Revenue](https://experienceleague.adobe.com/docs/analytics/components/metrics/revenue.html)
* [Orders](https://experienceleague.adobe.com/docs/analytics/components/metrics/orders.html?lang=en)
* [Units](https://experienceleague.adobe.com/docs/analytics/components/metrics/units.html?lang=en)
* [Carts](https://experienceleague.adobe.com/docs/analytics/components/metrics/carts.html?lang=en)
* [Cart Views](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-views.html)
* [Checkouts](https://experienceleague.adobe.com/docs/analytics/components/metrics/checkouts.html)
* [Cart Additions](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-additions.html)
* [Cart Removals](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-removals.html)

### Custom Conversion Metrics

* These metrics are specific to the report suite, so the available metrics vary for each customer and report suite.

### Reserved Conversion Metrics

* These metrics are specific to the report suite, so the available metrics vary for each customer and report suite.

>[!MORELIKETHIS]
>
>* [Overview of Analytics for Advertising Cloud](overview.md)
>* [Advertising Cloud Metrics in Analysis Workspace](/help/dsp/integrations/analytics/advertising-cloud-metrics-in-analytics.md)
