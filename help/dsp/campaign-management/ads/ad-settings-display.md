---
title: Display Ad Settings
description: Display Ad Settings
---

# Display Ad Settings

The following settings are for standard display ads. You can also serve click-to-play video ads for display ads, but we don't recommend doing so because not many publishers support them.

## Ad Options

### Basic

**Ad Type:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached. It defaults to *Display*.

**Ad Name:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 300x250 Gamer”).

**\[Ad Source\]**: Whether Advertising Cloud DSP is serving the ad (*Adobe served*) or you're using a third-party ad server (*3rd party*).

**This is an expandable Banner:** (Third-party ads only) Indicates the ad is an expandable banner ad. The related expansion settings determine which inventory to buy, so make sure they reflect the ad behavior.

**Expansion Method:** (Third-party expandable banner ads only) Whether the banner expands upon *Click* or *Rollover*.

**Expansion Directions:** (Third-party expandable banner ads only) The direction in which the ad expands: *Up*, *Down*, *Left*, or *Right*.

**Certified Vendors:** (Third-party expandable banner ads only) The certified vendor for which the ad is available: *DCM* (Google DoubleClick for Advertisers), *Flashtalking*, *Sizmek*, or *Jivox*.

**Display Code:** (Third-party ads only) The URL of the third-party creative asset. Any [timestamp] and [[timestamp]] parameters will be replaced with actual values.

**Final Display Code:** (Third-party ads only) The URL for the third-party creative asset, with the necessary Advertising Cloud tracking macros inserted, if applicable.

**Creative type:** (Adobe-served ads only) Whether the asset is an *Image* or an *HTML5* asset.

**Asset | HTML5 Asset:** (Adobe-served ads only) An image file or zipped HTML5 asset to upload, depending on the creative type. Click **Browse** and locate the file on your device or network, and then click **Upload** or **Upload Image**.

**Ad Size:** The width and height of the ad. It must be a [supported standard display ad size](/help/dsp/assets/ad-specs.pdf). You can manually enter the ad size before you upload the ad or enter a Display Code. If you don't enter the ad size, the dimensions of the uploaded ad or ad tag are automatically entered as read-only. Note that the Display ad will not save if the dimensions are not within Standard Display as sizes - e.g. 301x250 instead of 300x250 ad size.

>[!IMPORTANT]
>
> The ad size declared in the width and height fields will be matched with incoming bid requests. You may experience delivery issues if the ad's dimensions don't match the declared ad size.

**Click URL:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**Final Click URL:** (Adobe-served ads only; read-only) The Click URL with the necessary Advertising Cloud tracking macros inserted, if applicable.

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
