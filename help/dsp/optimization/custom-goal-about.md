---
title: About Custom Goals
description: About Custom Goals
exl-id: 623cb1ef-85ab-4535-aa3a-8e6ec8ae15ee
---
# About Custom Goals

Custom goals define the success events that an advertiser requires to meet its business objectives. Each package that uses the optimization goals "Highest ROAS - Custom Goal" or "Lowest CPA - Custom Goal" must include a custom goal that will help achieve the overall optimization goal. You can create custom goals as *objectives* in Advertising Cloud Search.

![custom goals](/help/dsp/assets/objective-goals.png)

Each custom goal consists of one or more metrics, or *transaction properties*, and the relative weights of those transaction properties. The available transaction properties include all metrics tracked using the Advertising Cloud conversion pixel and through Adobe Analytics.

>[!NOTE]
>
>* Analytics dimensions and segments aren't available for Advertising Cloud optimization.
>* To use Analytics events in DSP, work with your Adobe account manager to configure an advertiser-level integration.
>* Analytics custom events follow this naming convention: `custom_event_[*event #*]_[*Analytics report suite ID*]`. Example: `custom_event_16_examplersid`

For example, suppose that three metrics (transaction properties) are relevant to a specific package in one of your campaigns: "PDF Download" valued at 20 USD, "Email Signup" valued at 30 USD, and "Order Confirmation" valued at 40 USD. If you want to give weight according to the one-time monetary value of the customer action, then the relative weights of the properties would be 1, 2, and 1.5.

See the [best practices for creating custom goals](custom-goal-best-practices.md) for tips on how to configure your custom goals.

Once you [create a custom goal](custom-goal-create.md), you can [assign it to a package](/help/dsp/campaign-management/packages/package-settings.md) for reporting and algorithmic optimization using Adobe Sensei.

>[!MORELIKETHIS]
>
>* [Create a Custom Goal](custom-goal-create.md)
>* [Best Practices for Building a Custom Goal](custom-goal-best-practices.md)
>* [Optimization Goals and How to Use Them](optimization-goals.md)
>* [Package Settings](/help/dsp/campaign-management/packages/package-settings.md)
> * [How DSP Optimizes Your Campaigns](optimization-how-dsp-optimizes-campaigns.md)
