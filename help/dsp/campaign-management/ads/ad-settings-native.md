---
title: Native Ad Settings
description: See descriptions of the available ad settings for native ads.
feature: DSP Ads
exl-id: 3ae59e63-ae64-41b2-8734-3df2da020c7c
---
# Native Ad Settings

## [!UICONTROL Upload or Select Creative]

*New video (but not display) ads only*

**[!UICONTROL Upload Audio]:** To upload a raw asset to DSP. When you select this, do the following:

1. Click **[!UICONTROL Choose File]** and locate the file on your device or network.
1. Enter a title for the file, which will be used in the [!UICONTROL Ads] view and reports.
1. Click **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Audio]:** To select any previously-uploaded creative in the correct format within the account.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**[!UICONTROL Ad Name]:** The ad name. The ad type (display native) or video title (video formats) is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the [!UICONTROL Ads] view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 15sec Native”).

**[!UICONTROL Native Creative]:** A 1200x627 image to maximize delivery on mobile inventory. For video ads, this will be the image displayed before the Native video plays. Click **[!UICONTROL Browse]** and locate the file on your device or network, and then click **[!UICONTROL Upload]**.

**[!UICONTROL Title]:** An eye-catching title that will engage viewers.

**[!UICONTROL Description]:** For video ads, this is a short summary of the ad. For display ads, this is the body of the ad. The maximum length is 100 characters.

**[!UICONTROL Landing Page]:** The URL on which the viewer will land when they click the ad.

**[!UICONTROL Final Landing Page]:** The [!UICONTROL Landing Page] URL with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL Sponsored By (Advertiser Name)]:** The advertiser for the ad.

**[!UICONTROL Call to Action]:** (Optional) The step you want viewers to take once they see this ad.

**[!UICONTROL Advertiser Logo]:** (Optional) A 1:1 ratio logo to include with the ad for more brand recognition. Click **[!UICONTROL Browse]** and locate the file on your device or network, and then click **[!UICONTROL Upload]**.

### [!UICONTROL Pixel]

All existing event tracking pixels for the placement are automatically attached. You can detach existing pixels and create new pixels as needed, based on your tracking needs.

The following settings apply to each pixel that you create or edit.

**[!UICONTROL Integration Event]:** The event that triggers the pixel to fire. For this ad type, use pixels that fires on the *[!UICONTROL Impression]* or *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Whether the pixel is an *[!UICONTROL IMG URL]* (1x1 pixel image file), *[!UICONTROL HTML]*, or *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** The URL of the pixel image, in the appropriate format for the specified [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** The pixel name. Use a name that will help you easily identify the pixel.

**[!UICONTROL Pixel Provider]:** The pixel provider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, or *[!UICONTROL Comscore]*.

>[!MORELIKETHIS]
>
>* [About Ad Management](ad-about.md)
>* [Create an Ad](ad-create.md)
>* [List the Placements Associated with an Ad](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)
