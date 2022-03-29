---
title: Mobile Ad Settings
description: See descriptions of the available ad settings for mobile ads.
feature: DSP Ads
exl-id: f67c4ba0-1011-4ad6-bd36-98c312b81b67
---
# Mobile Ad Settings

## [!UICONTROL Insert Ad Tag]

*New mobile video ads formats only*

**[!UICONTROL Vertical video]:** (Not available when [!UICONTROL Custom Transcode] is selected) Indicates that the video is vertical (portrait mode).

**[!UICONTROL Transcode to]:** (Some users, depending on permissions; optional) The formats you want to include in your VAST tag when the publisher has specific creative file requirements. Formats accepted by most publishers are selected by default.

**[!UICONTROL Custom Transcode]:** (Beta users only; not available when Vertical Video is selected) ) Indicates that the video uses custom transcode. If you select this option, then specify the file format, video bitrate, zoom, and dimensions for up to three custom transcode versions.

**[!UICONTROL XTrader]:** (Some users, depending on permissions) Indicates that the video uses one ore more [!DNL X_TRADER] feed.

**[!UICONTROL Advanced: VAST Tag URL]:** (Some ad types) To enter a third-party VAST tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **[!UICONTROL Advanced: VAST Tag URL]**.
1. In the **[!UICONTROL URL]** field, enter the VAST tag URL.
1. Enter a **[!UICONTROL Title]** for the file, which will be used in the [!UICONTROL Ads] view and reports.

>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **[!UICONTROL Enter]** key. If the tag is valid, you will see an XML file that includes `<VAST>` near the top.

**[!UICONTROL Advanced: 3rd party Ad Tag]:** (Some ad types) To enter a third-party ad tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **[!UICONTROL Advanced: #3rd party Ad Tag]**.
1. Enter an **[!UICONTROL Ad Title]** for the file, which will be used in the [!UICONTROL Ads] view and reports.
1. In the **[!UICONTROL Ad Tag]** field, enter the ad tag.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]: Mobile Display Ads

**[!UICONTROL Ad Type]:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**[!UICONTROL Ad Name]:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 300x250 Gamer”).

**\[Ad Source\]**: Whether Advertising Cloud DSP is serving the ad (*[!UICONTROL Adobe served]*) or you're using a third-party ad server (*[!UICONTROL 3rd party]*).

**[!UICONTROL Creative type]:** (Adobe-served ads only) Whether the asset is an *[!UICONTROL Image]* or an *[!UICONTROL HTML5]* asset.

**[!UICONTROL Asset] | [!UICONTROL HTML5 Asset]:** (Adobe-served ads only) An image file or zipped HTML5 asset to upload, depending on the creative type. Click **[!UICONTROL Browse]** and locate the file on your device or network, and then click **[!UICONTROL Upload]**.

**[!UICONTROL Click URL]:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**[!UICONTROL Final Click URL]:** (Adobe-served ads only; read-only) The Click URL with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL Display Code]:** (Third-party ads only) The URL of the third-party creative asset. Any [timestamp] and [[timestamp]] parameters will be replaced with actual values.

**[!UICONTROL Final Display Code]:** (Third-party ads only) The URL for the third-party creative asset, with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

### [!UICONTROL Basic]: Video Ads

**[!UICONTROL Ad Type]:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**[!UICONTROL Ad Name]:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 30sec Phone Preroll”).

**[!UICONTROL Width] | [!UICONTROL Ad Unit Width]:** The width of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

**[!UICONTROL Height] | [!UICONTROL Ad Unit Height]:** The height of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

**[!UICONTROL Player X]:** The X coordinate for the ad unit. Keep the default setting.

**[!UICONTROL Player Y]:** The Y coordinate for the ad unit. Keep the default setting.

**[!UICONTROL Player Width]:** The width of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

This is the same as the **[!UICONTROL Width]** field.

**[!UICONTROL Player Height]:** The height of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

This is the same as the **[!UICONTROL Height]** field.

**[!UICONTROL Show Controls]:** Where to include video controls for the ad: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]*, or *[!UICONTROL None]* (the default).

**[!UICONTROL Preserve Aspect Ratio]:** Whether to to keep the video's width and height proportions (*[!UICONTROL Yes]*) or to stretch the video to fill available space (*[!UICONTROL No]*).

**[!UICONTROL Close Button Delay]:** (Some ad types) The number of seconds to delay the appearance of the close button.

**[!UICONTROL Click URL]:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**[!UICONTROL Final Click URL]:** (Adobe-served ads only; read-only) The [!UICONTROL Click URL] with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL VAST Tag]:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the creative asset.

**[!UICONTROL Final VAST Tag]:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the creative asset with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**[!UICONTROL Wmode]:** (Some ad types) The window mode: *[!UICONTROL window]*, *[!UICONTROL transparent]*, or *[!UICONTROL opaque]*.

### [!UICONTROL Pixel]

All existing event tracking pixels for the placement are automatically attached. You can detach existing pixels and create new pixels as needed, based on your tracking needs.

The following settings apply to each pixel that you create or edit.

**[!UICONTROL Integration Event]:** The event that triggers the pixel to fire. For this ad type, use pixels that fires on the *[!UICONTROL Impression]* or *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** Whether the pixel is an *[!UICONTROL IMG URL]* (1x1 pixel image file), *[!UICONTROL HTML]*, or *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** The URL of the pixel image, in the appropriate format for the specified [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** The pixel name. Use a name that will help you easily identify the pixel.

**[!UICONTROL Pixel Provider]:** The pixel provider: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, or *[!UICONTROL Comscore]*.

### [!UICONTROL Sharing]

Deprecated

>[!MORELIKETHIS]
>
>* [About Ad Management](ad-about.md)
>* [Create a Single Third-party Ad](ad-create.md)
>* [List the Placements Associated with an Ad](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)
