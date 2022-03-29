---
title: Audio Ad Settings
description: See descriptions of the available ad settings for audio ads.
feature: DSP Ads
exl-id: 746b6f40-ff59-4bbe-bfc0-3579d4461e4a
---
# Audio Ad Settings

## [!UICONTROL Insert Ad Tag]

*New ads only*

**[!UICONTROL Upload Audio]:** To upload a raw asset to DSP. When you select this, do the following:

1. Click **[!UICONTROL Choose File]** and locate the file on your device or network.
1. Enter a title for the file, which will be used in the [!UICONTROL Ads] view and reports.
1. Click **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Audio]:** To select any previously-uploaded creative in the correct format within the account.

**[!UICONTROL Advanced: VAST Tag URL]:** To enter a third-party VAST tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **[!UICONTROL Advanced: VAST Tag URL]**.
1. In the **[!UICONTROL URL]** field, enter the VAST tag URL.
1. Enter a **[!UICONTROL Title]** for the file, which will be used in the [!UICONTROL Ads] view and reports.

>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **[!UICONTROL Enter]** key. If the tag is valid, you will see an XML file that includes `<VAST>` near the top.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached. It defaults to *[!UICONTROL Audio]*.

**[!UICONTROL Ad Name]:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the [!UICONTROL Ads] view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 30sec Audio”).

**[!UICONTROL Ad Duration]:** The length of the audio file. It's automatically set as either [!UICONTROL 15] or [!UICONTROL 30], depending on the selected ad unit.

This field may or may not be displayed, depending on the account permissions.

**[!UICONTROL Click URL]:** (Ads using raw assets and with display banners only; optional) The URL on which the viewer will land when they click a display banner that accompanies your ad.

**[!UICONTROL Final Click URL]:** (Ads using raw assets and with display banners only; read-only) The [!UICONTROL Click URL] with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL VAST Tag]:** (Ads using VAST tags only) An URL for a third-party ad source. Make sure that the VAST tag includes only audio media files.

**[!UICONTROL Final VAST Tag]:** (Ads using VAST tags only) The URL for the third-party ad source with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL Select Rate]:** (Users with permission only) A pre-negotiated rate billed through Adobe, or one of the rates that you've negotiated and will be billed for through the vendor. To add a rate, contact your [!DNL Adobe] account team.

### Pixel

All existing event tracking pixels for the placement are automatically attached. You can detach existing pixels and create new pixels as needed, based on your tracking needs.

The following settings apply to each pixel that you create or edit.

**[!UICONTROL Integration Event]:** The event that triggers the pixel to fire. For this ad type, use pixels that fires on the *[!UICONTROL Impression]* or *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Whether the pixel is an *[!UICONTROL IMG UR]L* (1x1 pixel image file), *[!UICONTROL HTML]*, or *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** The URL of the pixel image, in the appropriate format for the specified Pixel Type.

**[!UICONTROL Pixel Name]:** The pixel name. Use a name that will help you easily identify the pixel.

**[!UICONTROL Pixel Provider]:** The pixel provider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, or *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [About Ad Management](ad-about.md)
>* [Create a Single Third-party Ad](ad-create.md)
>* [List the Placements Associated with an Ad](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)
