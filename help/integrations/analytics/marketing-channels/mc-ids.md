---
title: Using Advertising Cloud IDs to Create Marketing Channel Rules
description: Learn how to use Advertising Cloud IDs to create processing rules for Adobe Analytics Marketing Channels.
feature: Integration with Adobe Analytics
exl-id: 
---
# Using Advertising Cloud IDs to Create Marketing Channel Processing Rules

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

You can use Advertising Cloud IDs ([AMO ID and EF ID](../ids.md)) to configure Marketing Channel processing rules in Adobe Analytics. Use Advertising Cloud IDs for rules specific to your Advertising Cloud campaigns.

## The AMO ID in Processing Rules

The AMO ID is the primary tracking code used to report Advertising Cloud data within Analytics. The AMO ID is a concatenation of dynamic values managed by Adobe to provide granular reporting within Analytics. It's stored in an Analytics [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) or rVar dimension (AMO ID). The AMO ID can be set in Analytics in two ways:

* Click-through tracking: Advertising Cloud sets the s_kwcid query string parameter in a link, and Analytics picks up the parameter from the landing page URL when a click-through occurs.
* View-through tracking (DSP Only): The Last Event Service detects a view-through on the server side and sends the AMO ID to Analytics. In this case, the URL doesn't contain a s_kwcid parameter.

The dynamic values within AMO IDs indicate the marketing channel that was tracked:

* The prefix in the AMO ID can be used to identify the top-level channel within Marketing Channels.

* Character phrases in the body of the AMO ID indicate a more specific campaign type.

* The suffix “vt” is present for DSP view-through traffic and can be used to create separate click-through and view-through DSP channels.

The rest of the AMO ID can be ignored.

| AMO ID | Channel | Rule Logic |
|--------|---------|--------------------|
| AL! (prefix) | Paid Search | Starts With |
| AC! (prefix) | DSP | Starts With |
| !g! (body) | Google Search | Contains |
| !s! (body) | Search Partner | Contains |
| !d! (body) | Display Network | Contains |
| !u! (body) | Smart Shopping Campaign | Contains |
| !ytv! (body) | YouTube Video Ad | Contains |
| !yts! (body) | YouTube Search Ad | Contains |
| !vp! (body) | Google Video Partners | Contains |
| !vt (suffix) | DSP View-through | Ends With |

### Examples of Processing Rules That Use the AMO ID

The Marketing Channel Processing rule for the “Paid Search” channel might look like this:

![Example of a Paid Search rule](/help/integrations/assets/a4adc-mc-rule-paidsearch.png)

The Marketing Channel Processing rule for the “YouTube Video Ads” channel might look like this:

![Example of a YouTube video ads rule](/help/integrations/assets/a4adc-mc-rule-youtube-video.png)

>[!IMPORTANT]
>
> Be sure to run your rules in order of specificity. If the above two rules ran in order, the YouTube video ad traffic would all fall under the Paid Search channel because the AMO ID would both start with “AL!” and contain “!ytv!”.

## The AMO EF ID in Processing Rules

The AMO EF ID (EF ID) is the second tracking code used in the Analytics for Advertising Cloud integration. Its primary purpose is to track and pass Analytics event data into Advertising Cloud. Every time a click-through or a view-through occurs, a unique EF ID is generated, even if it is the exact same ad for the same visitor. The EF ID is not used in the Analytics reporting UI because it typically exceeds the 500k unique values per variable limit in Analytics, making it unusable for reporting. The Advertising Cloud metrics and metadata are not applied to the AMO EF ID; they are applied only to the AMO ID. The added granularity of tracking is required for campaign optimization in Advertising Cloud, so both IDs are required.

Although the AMO EF ID dimension isn't used directly in Analytics reporting, the EF ID can be useful in creating marketing channels. The EF ID suffix indicates the channel (display or search) and whether the visit was driven by a click-through or a view-through. The delimiter in the EF ID is a colon, rather than the exclamation point in the AMO ID.

| EF_id Suffix | Channel |
|-------|---------|
| :s | Paid Search |
| :d | Display Click-through |
| :i | Display View-through |

### Examples of Processing Rules That Use the AMO EF ID

#### Display Click-through Rule

Create a Display click-through marketing channel by capturing only click-throughs. Because the AMO ID is the same for both click-throughs and view-throughs, this rule uses the AMO EF ID variable and the ef_id query string parameter.

Sometimes click-throughs are tracked through the URL (the default). In other cases, click-throughs are tracked through the Last Event Service on the server side, and therefore the URL doesn't contain the ef_id parameter. The rule therefore checks for conditions in which the AMO EF ID variable or the ef_id query string parameter ends with “:d”. Use the "Any" operator because you want this rule to be triggered for either condition.

![Example of a display click-through rule](/help/integrations/assets/a4adc-mc-rule-display-ct.png)

#### Display View-through Rule

To create a Display view-through channel, create a rule in which the AMO EF ID ends with “:i”. Because the visitor didn't click the ad, the view-through tracking doesn't include the ef_id or s_kwcid in the URL. Therefore, only one condition is needed.

![Example of a display view-through rule](/help/integrations/assets/a4adc-mc-rule-display-vt.png)

>[!MORELIKETHIS]
>
>* [Fundamentals of Adobe Analytics Marketing Channels](mc-overview.md)
>* [Why Channel Data Can Vary Between Advertising Cloud and Marketing Channels](mc-data-variances.md)
>* [Using Adobe Analytics Marketing Channels with Advertising Cloud Data](mc-ac-data.md)
>* [Video: Reporting with Advertising Cloud Marketing Channels](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Advertising Cloud IDs Used by Analytics](/help/integrations/analytics/ids.md)
