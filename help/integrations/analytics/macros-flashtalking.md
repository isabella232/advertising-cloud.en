---
title: Configure Flashtalking Tags with Macros to Capture AMO IDs and Other Data
description: Learn how to add Analytics for Advertising Cloud macros to Flashtalking ad tags<!-- ??? -->
feature: Integration with Adobe Analytics
---
# Configure Flashtalking Tags with Macros to Capture AMO IDs and Other Data

<!-- This doesn't apply specifically to Analytics for Advertising Cloud; it can also apply to any type of Analytics integration?  Or should this be in a generic "Tracking" chapter of DSP help (or a cross-product chapter)? -->

<!-- Joe has links to internal docs, and one on Document Cloud that maybe is meant to be external-facing (?) but doesn't work. -->

*Advertisers with Flashtalking ads*

The following types of advertisers should use macros to capture AMO Ids and other data for Flashtalking display and video ads:

* **Advertisers with the [!DNL Adobe] [!DNL Analytics for Advertising Cloud] JavaScript code implemented on their websites**: You should see some click-through data in Adobe Analytics from ads you buy through Advertising Cloud, without extra macros. To capture additional click-through data that isn't captured through the JavaScript code<!-- give example of what that might include-->, though, add the macros in the following sections to your Flashtalking ad tags.

>[!NOTE]
>
>The JavaScript code is a solution for click tracking only while cookies are still available. Once Advertising Cloud discontinues cookies, implementing the following macros will be necessary.

* For advertisers whose websites don't use the [!DNL Analytics for Advertising Cloud] JavaScript code and instead rely on Adobe Analytics server-side forwarding for click-through data only (without any view-through data), then the following macros are required to report onsite click activity driven from ads you buy through Advertising Cloud.

## Display Ad Tags

Append the following macro to the end of the click-through URL in the `Clicktag` field:

```html
?[ftqs:[AdobeAMO]]
```

Example:  `https://www.adobe.com/products/photoshop?[ftqs:[AdobeAMO]]`

![Example of [!DNL Flashtalking] ad tag settings](/help/integrations/assets/macro-flashtalking-display-ad.png)

## Video Ad Tags

Append the following macro to the end of the click-through URL in the `Clicktag` field:

```html
?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]
```

Example:  `https://www.adobe.com/products/photoshop?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]`

![Example of [!DNL Flashtalking] ad tag settings](/help/integrations/assets/macro-flashtalking-video-ad.png)
