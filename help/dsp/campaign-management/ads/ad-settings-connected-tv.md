---
title: Connected TV Ad Settings
description: See descriptions of the available ad settings for connected TV ads.
feature: campaign management, ads, connected TV
exl-id: 4daae9e4-27eb-4496-9186-f33aebd8daae
---
# Connected TV Ad Settings

## Upload or Select Creative

*New ads only*

**Upload Audio:** To upload a raw asset to DSP. When you select this, do the following:

1. Click **Choose File** and locate the file on your device or network.
1. Enter a title for the file, which will be used in the Ads view and reports.
1. Click **Upload**.

**Use Existing Audio:** To select any previously-uploaded creative in the correct format within the account.

**Advanced: VAST Tag URL:** (Some ad types) To enter a third-party VAST tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **Advanced: VAST Tag URL**.
1. In the **URL** field, enter the VAST tag URL.
1. Enter a **Title** for the file, which will be used in the Ads view and reports.

>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **Enter** key. If the tag is valid, you will see an XML file that includes `<VAST>` near the top.

## Ad Options

### Basic

**Ad Type:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**Ad Name:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 30sec CTV”).

**Width | Ad Unit Width:** The width of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

**Height | Ad Unit Height:** The height of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

**Player X:** The X coordinate for the ad unit. Keep the default setting.

**Player Y:** The Y coordinate for the ad unit. Keep the default setting.

**Player Width:** The width of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

This is the same as the **Width** field.

**Player Height:** The height of the entire ad unit. This option may be locked depending on the type of ad unit you selected.

This is the same as the **Height** field.

**Show Controls:** Where to include video controls for the ad: *Under*, *Over*, *Bottom*, or *None* (the default).

**Preserve Aspect Ratio:** Whether to to keep the video's width and height proportions (*Yes*) or to stretch the video to fill available space (*No*).

**Click URL:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**Final Click URL:** (Adobe-served ads only; read-only) The Click URL with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**VAST Tag:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the ad source.

**Final VAST Tag:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the ad source with the necessary [Advertising Cloud DSP tracking macros](/help/dsp/campaign-management/macros.md) inserted, if applicable.

**Clock Number**: (Used only in the United Kingdom; available only to users with permission) A unique identifier used to ensure that the right ad is broadcast. If this setting isn't applicable, leave it blank.

### Pixel

All existing event tracking pixels for the placement are automatically attached. You can detach existing pixels and create new pixels as needed, based on your tracking needs.

The following settings apply to each pixel that you create or edit.

**Integration Event:** The event that triggers the pixel to fire. For this ad type, use pixels that fires on the *Impression* or *Click-through*.

**Pixel Type:** Whether the pixel is an *IMG URL* (1x1 pixel image file), *HTML*, or *JavaScript URL*.

**Pixel URL or Code:** The URL of the pixel image, in the appropriate format for the specified Pixel Type.

**Pixel Name:** The pixel name. Use a name that will help you easily identify the pixel.

**Pixel Provider:** The pixel provider: *None*, *Nielsen*, or *Comscore*.

>[!MORELIKETHIS]
>
>* [About Ad Management](ad-about.md)
>* [Create an Ad](ad-create.md)
>* [List the Placements Associated with an Ad](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
>* [Advertising Cloud DSP Macros](/help/dsp/campaign-management/macros.md)
