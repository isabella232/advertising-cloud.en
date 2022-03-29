---
title: Pre-roll Ad Settings
description: See descriptions of the available ad settings for pre-roll ads.
feature: DSP Ads
exl-id: 638d5a3d-3dff-40b6-a3ba-7ab3f08282b9
---
# Pre-roll Ad Settings

## [!UICONTROL Insert Ad Tag]

*New ads only*

**[!UICONTROL Transcode to]:** (Some users, depending on permissions; optional) The formats you want to include in your VAST tag when the publisher has specific creative file requirements. Formats accepted by most publishers are selected by default.

**[!UICONTROL Custom Transcode]:** (Beta users only; not available when Vertical Video is selected) ) Indicates that the video uses custom transcode. If you select this option, then specify the file format, video bitrate, zoom, and dimensions for up to three custom transcode versions.

**[!UICONTROL XTrader]:** (Some users, depending on permissions) Indicates that the video uses one or more [!DNL X_TRADER] feed.

**[!UICONTROL Advanced: URL]:** (Some ad types) The VAST tag URL.

**[!UICONTROL Title]:** A title for the file, which will be used in the [!UICONTROL Ads] view and reports.

<!-- I think "Go" checks the validity.
>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **[!UICONTROL Enter]** key. If the tag is valid, you will see an XML file that includes `<VAST>` near the top.
-->

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**[!UICONTROL Ad Name]:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the [!UICONTROL Ads] view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 30sec Preroll”).

**[!UICONTROL Width] | [!UICONTROL Ad Unit Width]:** (Standard and skippable pre-roll ads only) The width of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

**[!UICONTROL Height] | [!UICONTROL Ad Unit Height]:** (Standard and skippable pre-roll ads only) The height of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

**[!UICONTROL Player X]:** The X coordinate for the ad unit. Keep the default setting.

**[!UICONTROL Player Y]:** The Y coordinate for the ad unit. Keep the default setting.

**[!UICONTROL Player Width]:** The width of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

This is the same as the **[!UICONTROL Width]** field.

**[!UICONTROL Player Height]:** The height of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

This is the same as the **[!UICONTROL Height]** field.

**[!UICONTROL Show Controls]:** Where to include video controls for the ad: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]*, or *[!UICONTROL None]* (the default).

**[!UICONTROL Preserve Aspect Ratio]:** Whether to to keep the video's width and height proportions (*[!UICONTROL Yes]*) or to stretch the video to fill available space (*[!UICONTROL No]*).

**[!UICONTROL Click URL]:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**[!UICONTROL Final Click URL]:** (Adobe-served ads only; read-only) The [!UICONTROL Click URL] with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL VAST Tag]:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the ad source.

**[!UICONTROL Final VAST Tag]:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the ad source with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL Wmode]:** (Interactive pre-roll only) The window mode: *[!UICONTROL window]*, *[!UICONTROL transparent]*, or *[!UICONTROL opaque]*.

**[!UICONTROL Video Format]:** (Interactive pre-roll only) The format of the ad player for potential inventory: *[!UICONTROL VPAID]* or *[!UICONTROL VPAID & VAST]*. Viewability is always measured for VPAID, but VPAID & VAST includes inventory that doesn’t allow viewability measurement. Keep this in mind if viewability metrics are important to your campaign.

**[!UICONTROL Clock Number]**: (Interactive pre-roll only; used only in the United Kingdom; available only to users with permission) A unique identifier used to ensure that the right ad is broadcast. If this setting isn't applicable, leave it blank.

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
>* [Create a Single Third-party Ad](ad-create.md)
>* [List the Placements Associated with an Ad](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)
