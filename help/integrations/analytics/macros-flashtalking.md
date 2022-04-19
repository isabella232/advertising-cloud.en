---
title: Append [!DNL Analytics for Advertising Cloud] Macros to [!DNL Flashtalking] Ad Tags
description: Learn why and how to add [!DNL Analytics for Advertising Cloud] macros to your [!DNL Flashtalking] ad tags
feature: Integration with Adobe Analytics
---
# Append [!DNL Analytics for Advertising Cloud] Macros to [!DNL Flashtalking] Ad Tags

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

*Applicable to Advertising Cloud DSP only*

If you use ad tags from [!DNL Flashtalking] for your Advertising Cloud DSP ads, append Analytics for Advertising Cloud parameters to your landing page URLs. The parameters allow Advertising Cloud to send click data for the ads to Adobe Analytics.

Use macros for [!DNL Flashtalking] display and video ads for the following types of [!DNL Analytics for Advertising Cloud] implementations:

* **Advertisers with the [!DNL Adobe] [!DNL Analytics for Advertising Cloud] JavaScript code implemented on their websites**: You should see some click-through data in Adobe Analytics from ads you buy through Advertising Cloud, without extra macros. To capture click-through data in browsers that don't support third-party cookies and therefore isn't captured through the JavaScript code, though, add the macros in the following sections to your [!DNL Flashtalking] ad tags.

>[!NOTE]
>
>The JavaScript code is a solution for click tracking only while cookies are still available. Once Advertising Cloud discontinues cookies, implementing the following macros will be necessary.

* **Advertisers whose websites don't use the [!DNL Analytics for Advertising Cloud] JavaScript code and instead rely on [!DNL Analytics] server-side forwarding for click-through data only** (without any view-through data): The following macros are required to report onsite click activity driven from ads you buy through Advertising Cloud.

## Display Ad Tags

Within the [!DNL Flashtalking] ad tag settings, append the following macro to the end of the click-through URL in the `Clicktag` field:

```html
?[ftqs:[AdobeAMO]]
```

Example:  `https://www.adobe.com/products/photoshop?[ftqs:[AdobeAMO]]`

![Example of [!DNL Flashtalking] ad tag settings](/help/integrations/assets/macro-flashtalking-display-ad.png)

## Video Ad Tags

Within the [!DNL Flashtalking] ad tag settings, append the following macro to the end of the click-through URL in the `Clicktag` field:

```html
?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]
```

Example:  `https://www.adobe.com/products/photoshop?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]`

![Example of [!DNL Flashtalking] ad tag settings](/help/integrations/assets/macro-flashtalking-video-ad.png)

>[!MORELIKETHIS]
>
>* [Overview of [!DNL Analytics for Advertising Cloud]](overview.md)

<!-- >* [Append [!DNL Analytics for Advertising Cloud] Macros to [!DNL Google Campaign Manager 360] Ad Tags](macros-google-campaign-manager.md) -->
