# Audio Ad Settings {#ad-settings-audio}

## Upload or Select Creative

*New ads only*

**Upload Audio:** To upload a raw asset to DSP. When you select this, do the following:

1. Click **Choose File** and locate the file on your device or network.
1. Enter a title for the file, which will be used in the Ads view and reports.
1. Click **Upload**.

**Use Existing Audio:** To select any previously-uploaded creative in the correct format within the account.

**Advanced: VAST Tag URL:** To enter a third-party VAST tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **Advanced: VAST Tag URL**.
1. In the **URL** field, enter the VAST tag URL.
1. Enter a **Title** for the file, which will be used in the Ads view and reports.

>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **Enter** key. If the tag is valid, you will see an XML file that includes <VAST> near the top.

## Ad Options

### Basic

**Ad Type:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached. It defaults to *Audio*.

**Ad Name:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 30sec Audio”).

**Ad Duration:** The length of the audio file. It's automatically set as either 15 or 30, depending on the selected ad unit.

This field may or may not be displayed, depending on the account permissions.

**Click URL:** (Ads using raw assets and with display banners only; optional) The URL on which the viewer will land when they click a display banner that accompanies your ad.

**Final Click URL:** (Ads using raw assets and with display banners only; read-only) The Click URL with the necessary Advertising Cloud tracking macros inserted, if applicable.

**VAST Tag:** (Ads using VAST tags only) An URL for a third-party ad source. Make sure that the VAST tag includes only audio media files.

**Final VAST Tag:** (Ads using VAST tags only) The URL for the third-party ad source with the necessary Advertising Cloud tracking macros inserted, if applicable.

**Select Rate:** (Users with permission only) A pre-negotiated rate billed through Adobe, or one of the rates that you've negotiated and will be billed for through the vendor. To add a rate, contact your Adobe account manager.

### Companion

*DSP-served ads only*

You can optionally attach up to three companion banners with an ad. The best practice is to attach companion banners where possible.

>[!NOTE]
>
>* Not all publishers allow companion banners. The publishers who do allow companion banners don't guarantee companion banner impressions.
>* Companion banners from third-party ad tags may not always available for preview.

**[Check Box]:** Includes the specified companion banner with the ad. When the check box is disabled, the companion banner isn't included.

**[Banner Size]:** The companion banner size: *300x250* (used for iHeartRadio, Spotify, SoundCloud, and TuneIn), *640x640* (used for Spotify), or *1024x1024* (used for SoundCloud).

**[Source]:** The source of the companion banner asset:

* *Upload My Own Asset:* To upload your own asset.
* *Use a Third Party Tag:* To enter an iFrame or script tag from a certified third-party ad serving partner.

Use a third-party tag when you want to track third-party companion banner impressions.

**Asset:** (Raw assets only) The companion banner asset, in GIF, JPG, or PNG format. Click **Browse** and locate the file on your device or network, and then click **Upload**.

**Click URL:** (Raw assets only) The URL on which the viewer will land when they click the companion banner for the ad. It can include a click redirect using a third-party click tracking pixel.

**Final Click URL:** (Raw assets only; read-only) The Click URL with the necessary Advertising Cloud tracking macros inserted, if applicable.

**Ad Tag:** (Ads using third-party ad tags only) An iFrame or script banner tag for a third-party companion banner source. It must be from a certified third-party ad serving partner.

**Final Ad Tag:** (Ads using third-party ad tags only) The Ad Tag with the necessary Advertising Cloud tracking macros inserted, if applicable.

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
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](https://education.tubemogul.com/wp-content/uploads/2020/08/Adobe_Avstg_Cloud-Ad-Specs-20201.pdf)
