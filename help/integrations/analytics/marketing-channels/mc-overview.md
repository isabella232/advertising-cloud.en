---
title: Fundamentals of Adobe Analytics Marketing Channels
description: Learn key information about Adobe Analytics Marketing Channels that Analytics for Advertising Cloud users should understand.
feature: integration with Adobe Analytics, Marketing Channels
exl-id: 
---
# Fundamentals of Adobe Analytics Marketing Channels

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

This page explains key information about Adobe Analytics Marketing Channels that Analytics for Advertising Cloud users need to understand.

For full documentation on Marketing Channels, see "[Get Started with Marketing Channels](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/c-getting-started-mchannel.html).

## Overview of Marketing Channels

Marketing Channels are a key feature of Adobe Analytics. Marketing Channels reports show how customers arrive to your website over the reporting window and how each channel impacts revenue or on-site behavior.

Consider the following example of a cross-visit journey. Each visit to your website is indicated by the Marketing Channel from which the visitor entered. The first visit, also referred to as the First Touch Channel, is Email. Display on visit two is a participating channel, and Natural Search is considered the Last Touch Channel. If you use Last Touch Attribution within Attribution IQ, Natural Search would receive full credit for the $250 conversion event. Using the Experience Cloud ID Service, you can tie these individual visits together to reveal one journey by a single visitor.

![Example cross-visit conversion journey in Marketing Channels](/help/integrations/assets/a4adc-mc-sample-journey.png)

By using Marketing Channel Processing Rules, you can create sets of logic to determine the channels that drive traffic and to track each channel as users comes to your site. For example, the Email channel would be indicated by a unique tracking code generated upon click that, when logged by Adobe Analytics, would categorize the visit as originating from an Email marketing campaign.

## Processing Rules and How Marketing Channels are Set

Each time a user comes to a website, they do so through a URL that they either clicked or directly typed into the address bar. When the user enters the website, Analytics tracks information that can be used to determine the channel that drove the visit.

Often, marketers append query string parameter tracking codes to channel URLs to help track the impact of the channel on their site. You can configure Marketing Channel processing rules to listen for specific tracking parameters and values to determine the channel without any additional tracking. For example, if all email campaign URLs follow the format `www.adobe.com?cid=email…` (where the URL contains the query string parameter and value ”cid=email”), then you can create a rule to listen for this tracking code and to bucket the visit in the Email channel.

Other channels don't have trackable URL paths and need further logic for identification. For example, Earned Social, in which a user clicks a link that another user shared organically on a social network, is an important channel to track. However, the marketer has no way to append a query string parameter tracking code to the URL that's shared. In this case, you could create a processing rule to listen for the referring domain of social networks of interest and the absence of paid tracking codes to determine the channel. The visits that meet these requirements would then be tracked as Earned Social within the Marketing Channels report.

Adobe recommends working with your analytics team to build a comprehensive set of Marketing Channel processing rules to track all channels that are pertinent to your business. Doing so allows you to create powerful attribution reporting.

To understand how Advertising Cloud can contribute to the signals necessary to create custom marketing channels, see "[Using Advertising IDs to Create Marketing Channel Rules](ids-in-mc-rules.md)."

>[!MORELIKETHIS]
>
>* [Using Advertising Cloud IDs to Create Marketing Channel Processing Rules](mc-ids.md)
>* [Why Channel Data Can Vary Between Advertising Cloud and Marketing Channels](mc-data-variances.md)
>* [Using Adobe Analytics Marketing Channels with Advertising Cloud Data](mc-ac-data.md)
>* [Video: Reporting with Advertising Cloud Marketing Channels](https://experienceleague.adobe.com/docs/advertising-cloud-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Overview of Analytics for Advertising Cloud](/help/integrations/analytics/overview.md)
