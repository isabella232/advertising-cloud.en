---
title: Pre-roll Ad Settings
description: See descriptions of the available ad settings for pre-roll ads.
feature: DSP Ads
exl-id: 638d5a3d-3dff-40b6-a3ba-7ab3f08282b9
---
# Pre-roll Ad Settings

## [!UICONTROL Upload or Select Creative]

*New ads only*

**[!UICONTROL Transcode to]:** (Some users, depending on permissions; optional) The formats you want to include in your VAST tag when the publisher has specific creative file requirements. Formats accepted by most publishers are selected by default.

**[!UICONTROL Custom Transcode]:** (Beta users only; not available when Vertical Video is selected) ) Indicates that the video uses custom transcode. If you select this option, then specify the file format, video bitrate, zoom, and dimensions for up to three custom transcode versions.

**[!UICONTROL XTrader]:** (Some users, depending on permissions) Indicates that the video uses one or more [!DNL X_TRADER] feed.

**[!UICONTROL Upload Video]:** To upload a raw asset to DSP. When you select this, do the following:

1. Click **[!UICONTROL Choose File]** and locate the file on your device or network.
1. Enter a title for the file, which will be used in the [!UICONTROL Ads] view and reports.
1. Click **[!UICONTROL Upload]**.

**[!UICONTROL Use Existing Video]:** To select any previously-uploaded creative in the correct format within the account.

**[!UICONTROL Advanced: VAST Tag URL]:** (Some ad types) To enter a third-party VAST tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **[!UICONTROL Advanced: VAST Tag URL]**.
1. In the **[!UICONTROL URL]** field, enter the VAST tag URL.
1. Enter a **[!UICONTROL Title]** for the file, which will be used in the [!UICONTROL Ads] view and reports.

>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **[!UICONTROL Enter]** key. If the tag is valid, you will see an XML file that includes `<VAST>` near the top.

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

### [!UICONTROL Companion]

*DSP-served ads only*

You can optionally attach up to three companion banners with an ad. The best practice is to attach companion banners where possible.

>[!NOTE]
>
> Not all publishers allow companion banners. The publishers who do allow companion banners don't guarantee companion banner impressions.
> Companion banners from third-party ad tags may not always available for preview.

**\[Check Box\]:** Includes the specified companion banner with the ad. When the check box is disabled, the companion banner isn't included.

**\[Banner Size\]:** The companion banner size: *[!UICONTROL 300x600 (Skyscraper)]*; *[!UICONTROL 300x250 (Medium Rectangle)]*, which is the most common ad size and recommended for all ads; *[!UICONTROL 300x60 (Small Banner)]*; or *[!UICONTROL 728x90 (Leaderboard)]*, which is a less common ad size.

**\[Source\]:** Whether you're uploading your own companion banner asset or using a third-party tag.

**Asset:** (Raw assets only) The companion banner asset. Click **[!UICONTROL Browse]** and locate the file on your device or network, and then click **[!UICONTROL Upload]**.

**Ad Tag]:[!UICONTROL ** (Ads using VAST tags only) An URL to a third-party companion banner source.

**[!UICONTROL Final Ad Tag]:** (Ads using VAST tags only) An URL to a third-party companion banner source source with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

### [!UICONTROL Overlays]

*Interactive pre-roll and mobile interactive and tap-to-play formats for DSP-served ads*

The following settings apply to each overlay that you create or edit.

**[!UICONTROL Asset]:** (Raw assets only) The overlay image asset. The file must be in single-frame GIF, JPG, or PNG format, and the maximum image size is less than 2MB. To upload the asset, click **[!UICONTROL Browse]** and locate the file on your device or network, and then click **[!UICONTROL Upload]**.

>[!TIP]
>
>See the [Best Practices for Designing Overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)

**[!UICONTROL Click URL]:**  The URL on which the viewer will land when they click an overlay for your ad.

**[!UICONTROL X]:** The X coordinate for the overlay. Select the overlay starting position, and then enter the number of pixels from the starting position (such as 10px From Center). The best practice is to use *From Center*, which prevents the overlay from moving around with different player sizes on publisher sites.

**[!UICONTROL Y]:** The Y coordinate for the overlay. Select the overlay starting position, and then enter the number of pixels from the starting position (such as 10px from Top). The best practice is specify a coordinate *[!UICONTROL From Bottom]* or *[!UICONTROL From Top],* depending the position in which you’d like the overlay to be displayed on the ad.

**[!UICONTROL Layer]:** The layer in which the overlay will appear. The video and each overlay will be in separate layers.

* *[!UICONTROL 2 through 5]:* In front of the video but behind other overlays.

* *[!UICONTROL 1]:* In front of the video.

* *[!UICONTROL 0]:* In the same layer as the video. The video will shrink to fill the remaining space. Not recommended for Interactive Preroll.

* *[!UICONTROL -1]:* Behind the video.

* *[!UICONTROL -2 through -5]:* Behind the video but in front of other overlays.

* *[!UICONTROL Background]:* Behind the video and other overlays. The overlay will scale to the full width and height of the video, and the aspect ratio won't be preserved.

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
>* [Best Practices for Designing Overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)
