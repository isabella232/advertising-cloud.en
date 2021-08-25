---
title: Why Channel Data Can Vary Between Advertising Cloud and [!DNL Marketing Channels]
description: Learn why channel data tracked by the AMO ID can vary from channel data tracked by [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
exl-id: 
---
# Why Channel Data Can Vary Between Advertising Cloud and [!DNL Marketing Channels]

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

A common question from users learning about the integration of the Advertising Cloud and [!DNL Marketing Channels] data sets is “What causes the variance in data between the AMO ID and [!DNL Marketing Channels]?” Or, sometimes, “Why is the data broken? I need all metrics to match across the reports.” Fortunately, discrepancies don't indicate that the data is "broken,” and discrepancies are expected and even desired. Let’s look at why the integration was designed this way.

The two data sets have different primary use cases:

* [!DNL Marketing Channels]: The primary use case for [!DNL Marketing Channels] is to compare data across multiple channels with a common attribution model. Analysts can use the Marketing Channel dimension to gain increased insights into how channels are interacting with each other. This insight can help fuel macro-level decisions on how to invest in each channel and can lead to insights on how visitors from each channel interact with the website.

     The [!DNL Analytics] Marketing Channel dimension, therefore, is configured to capture and track all channels. [!DNL Marketing Channels] can also be configured to capture Advertising Cloud DSP view-throughs and click-throughs, and it does so in relation to the other marketing channels.

* Advertising Cloud AMO ID: The primary use case of the Advertising Cloud AMO ID data is to feed Advertising Cloud’s advanced [!DNL Adobe Sensei]-powered bidding algorithms. The algorithms automatically make thousands of micro-level bid decisions made daily to maximize advertising spend and to achieve the goals of the [!DNL DSP] campaign or [!DNL Search] portfolio. The more conversion data the algorithms can connect campaigns to, the better the algorithms can make these bidding decisions.

     To collect this data, the [!DNL Analytics for Advertising Cloud] integration passes raw AMO IDs that can be translated as click-through and view-through tracking codes in the AMO ID dimension of Adobe Analytics &mdash; which is stored either as a custom variable (eVar) or a reserved variable (rVar). Click-throughs for other channels aren't set in the AMO ID dimension, so the AMO ID dimension is unable to track entry from these other channels. The result is that the AMO ID persists through [!DNL Marketing Channes]l entry points.

For more information about possible data variances between Advertising Cloud-tracked data and [!DNL Analytics]-tracked data, see "[Expected Data Variances Between [!DNL Analytics] and Advertising Cloud](../data-variances.md)."

>[!MORELIKETHIS]
>
>* [Expected Data Variances Between [!DNL Analytics] and Advertising Cloud](/help/integrations/analytics/data-variances.md)
>* [Fundamentals of [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Using Advertising Cloud IDs to Create [!DNL Marketing Channels] Processing Rules](mc-ids.md)
>* [Using [!DNL Analytics Marketing Channels] with Advertising Cloud Data](mc-ac-data.md)
>* [Video: Reporting with Advertising Cloud [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
