---
title: Prerequisites and Key Information for Implementing [!DNL Analytics for Advertising Cloud]
description: Prerequisites and Key Information for Implementing [!DNL Analytics for Advertising Cloud]
feature: Integration with Adobe Analytics
exl-id: 08e54e2b-ed9b-4489-8de5-ab1379b7133c
---
# Prerequisites and Key Information for Implementing [!DNL Analytics for Advertising Cloud]

*Advertisers with Advertising Cloud DSP and Advertising Cloud Search*

Review the following information before you integrate Advertising Cloud with Adobe Analytics.

## Requirements for Reporting Advertising Cloud Data in [!DNL Analytics]

* Experience Cloud Identity Service: `visitorAPI.js` version 2.0 or higher
* Any version of Adobe Analytics (including [!DNL Prime], [!DNL Premium], or [!DNL Ultimate])
* Adobe Analytics: `appMeasurement.js` version 2.1 or higher

>[!TIP]
>
>To improve data fidelity, use the most recent version of the Experience Cloud Identity Service with CNAME support, as well as the most recent version of Analytics AppMeasurement for JavaScript.

## Requirements for Sharing Analytics Segments with Advertising Cloud

* Experience Cloud Identity Service: `visitorAPI.js` version 2.1 or higher
* Adobe Analytics: `!DNL appMeasurement.js` version 1.8 or higher

## Requirements for Reporting [!DNL Analytics] Data in Advertising Cloud

Provide the Advertising Cloud implementation team with the following:

* The [!DNL Analytics] report suite ID that will be used for reporting on paid media activity and for feeding site activity for optimization and reporting in Advertising Cloud
* The company's Experience Cloud Organization ID (Org ID).

You can find both of these IDs on the [Summary screen of the Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/run-debugger.html).

![Experience Cloud Debugger Summary screen](/help/integrations/assets/a4adc-debugger-summary.png)

## [!DNL Analytics] Data in Advertising Cloud {#lookback-a4adc}

Because [!DNL Analytics] data is sent to Advertising Cloud for reporting and optimization, the data is subject to the attribution rules, including the impression and click lookback windows, that are configured for the advertiser in Advertising Cloud.

![advertiser-level lookback window settings in Advertising Cloud](/help/integrations/assets/a4adc-lookbacks.png)

* Advertising Cloud attribution click lookback window: The number of days after the first click occurs in which the click can be attributed to a conversion. By default, this value is 60 days; the maximum is 90 days  
* Advertising Cloud attribution impression lookback window: The number of days after an ad impression occurs in which the impression can be attributed to a conversion. By default, this value is 14 days; the maximum is 30 days

    >[!NOTE]
    >
    > The impression lookback window is specific to Advertising Cloud, not [!DNL Analytics for Advertising Cloud], reporting.

The [!DNL Analytics for Advertising Cloud] JavaScript uses these settings to determine how far back to consider a view-through entry or click-through entry to the site as valid. For more information about how view-throughs and click-throughs are determined, see "[Advertising Cloud IDs Used by Analytics](ids.md)."

## Advertising Cloud Data in [!DNL Analytics]

[!DNL Analytics] sets Advertising Cloud IDs (AMO IDs) within the Analytics hit, subject to the advertiser's eVar persistence setting, which applies to both click-throughs and view-throughs. The persistence setting is configured on the Advertising Cloud back end, and your Adobe account manager can change it.

* [!DNL Analytics for Advertising Cloud] eVar expiration: 60 days by default for AMO IDs

>[!NOTE]
>
>To segment data for a different timeframe, you can [set up custom segments](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html) with different lookback windows within Analysis Workspace.

## Supported Ad Environments

* Search
* Display
* Video
* Online Video
* Native

Contact your Adobe account manager for the latest supported ad environments in each channel.  

## Things to Know Before You Implement

* No additional costs are billed for this integration, nor do server calls result in additional [!DNL Analytics] or Advertising Cloud fees.

* [!DNL Analytics for Advertising Cloud] is ad server-agnostic: a view-through or click-through may occur from any ad server, and the proper IDs are generated upon site entry.

* The integration passes only [!DNL Analytics] standard and custom events to Advertising Cloud for bid optimization of subsequent paid media and advertising efforts. It doesn't pass [!DNL Analytics] segments, calculated metrics, and eVars to Advertising Cloud for bid optimization.

* Advertising Cloud creates persistent IDs within [!DNL Analytics] based on the last advertisement clicked or viewed before the user enters the site, based on the [click and view-through lookback windows](#lookback-a4adc) configured in Advertising Cloud. If a site visitor were to have both types of site entry interactions within their profile, and the click is within the lookback period, then the visitor's click-through ID would override the view-through ID for site reporting.

* [!DNL Analytics for Advertising Cloud] conversion tracking in Adobe Analytics uses a configurable tracking lookback window (60 days by default). Advertising Cloud reports reflect site conversions and engagement through the end of this tracking lookback window.

* All ad types are supported. However, not all ad environments are supported.

    For example, connected TV (CTV) ads aren't tracked because no clicks occur in CTV and no conversions can occur on the same device. However, if the ad is viewed within a desktop environment, then some view-through site entry data may be tracked.

* [!DNL Analytics] conversions are currently tracked and attributed only to a visitor on the same device.

* [!DNL Analytics for Advertising Cloud] doesn't support in-app view-through conversions.

* View-through tracking isn't supported for advertisers using a server-side forwarding implementation of [!DNL Analytics].

### Supplemental ID

Once the Experience Cloud Identity Service is implemented for a site, hits that contain data from [!DNL Analytics] or Advertising Cloud contain a supplemental ID.

Example: `sdid=2F3C18E511F618CC-45F83E994AEE93A0`

For accurate data integration, all Advertising Cloud calls used by an [!DNL Analytics for Advertising Cloud] activity to deliver content or record the goal metric must have a corresponding [!DNL Analytics] hit that shares the same supplemental ID.

When you're troubleshooting in [!DNL Analytics], be sure to confirm that the supplemental ID is present for [!DNL Analytics] hits. In the [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/experience-cloud-debugger.html), you can see this ID in the Advertising Cloud tab as the `sdid` parameter.

>[!NOTE]
>
> This implementation works similarly to the [!DNL Analytics] for Target] integration.

>[!MORELIKETHIS]
>
>* [Overview of [!DNL Analytics for Advertising Cloud]](overview.md)
>* [JavaScript Code for Analytics for Advertising Cloud](/help/integrations/analytics/javascript.md)
