# Mobile Ad Settings {#ad-settings-mobile}

## Upload or Select Creative

*New mobile video ads formats only*

**Vertical video:** (Not available when Custom Transcode is selected) Indicates that the video is vertical (portrait mode).

**Transcode to:** (Some users, depending on permissions; optional) The formats you want to include in your VAST tag when the publisher has specific creative file requirements. Formats accepted by most publishers are selected by default.

**Custom Transcode:** (Beta users only; not available when Vertical Video is selected) ) Indicates that the video uses custom transcode. If you select this option, then specify the file format, video bitrate, zoom, and dimensions for up to three custom transcode versions.

**XTrader:** (Some users, depending on permissions) Indicates that the video uses an X_TRADER feed(s).

**Upload Video:** To upload a raw asset to DSP. When you select this, do the following:

1. Click **Choose File** and locate the file on your device or network.
1. Enter a title for the file, which will be used in the Ads view and reports.
1. Click **Upload**.

**Use Existing Video:** To select any previously-uploaded creative in the correct format within the account.

**Advanced: VAST Tag URL:** (Some ad types) To enter a third-party VAST tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **Advanced: VAST Tag URL**.
1. In the **URL** field, enter the VAST tag URL.
1. Enter a **Title** for the file, which will be used in the Ads view and reports.

>[!TIP]
>
> To check the validity of a VAST tag, paste it into a browser and hit the **Enter** key. If the tag is valid, you will see an XML file that includes <VAST> near the top.

**Advanced: 3rd party Ad Tag:** (Some ad types) To enter a third-party ad tag that contains creative assets and tracking pixels:

1. Click ![arrow](/help/dsp/assets/compressed.png) next to **Advanced: #3rd party Ad Tag**.
1. Enter an **Ad Title** for the file, which will be used in the Ads view and reports.
1. In the **Ad Tag** field, enter the ad tag.

## Ad Options

### Basic: Mobile Display Ads

**Ad Type:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**Ad Name:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 300x250 Gamer”).

**[Ad Source]**: Whether Advertising Cloud DSP is serving the ad (*Adobe served*) or you're using a third-party ad server (*3rd party*).

**Creative type:** (Adobe-served ads only) Whether the asset is an *Image* or an *HTML5* asset.

**Asset | HTML5 Asset:** (Adobe-served ads only) An image file or zipped HTML5 asset to upload, depending on the creative type. Click **Browse** and locate the file on your device or network, and then click **Upload**.

**Click URL:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**Final Click URL:** (Adobe-served ads only; read-only) The Click URL with the necessary Advertising Cloud tracking macros inserted, if applicable.

**Display Code:** (Third-party ads only) The URL of the third-party creative asset. Any [timestamp] and [[timestamp]] parameters will be replaced with actual values.

**Final Display Code:** (Third-party ads only) The URL for the third-party creative asset, with the necessary Advertising Cloud tracking macros inserted, if applicable.

### Basic: Video Ads

**Ad Type:** (Read-only) The ad type you're creating, which corresponds to the placement type to which the ad can be attached.

**Ad Name:** The ad name. The asset title is used by default, but you can change the name.

>[!TIP]
>
> Use a name that will be easy to find when you attach the ad to a placement, in the Ads view, and in reports. For example, describe the unit type and some key attributes (such as Holiday Product Preview: 30sec Phone Preroll”).

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

**Close Button Delay:** (Some ad types) The number of seconds to delay the appearance of the close button.

**Click URL:** (Adobe-served ads only) The URL on which the viewer will land when they click the ad.

**Final Click URL:** (Adobe-served ads only; read-only) The Click URL with the necessary Advertising Cloud tracking macros inserted, if applicable.

**VAST Tag:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the creative asset.

**Final VAST Tag:** (Ads using VAST tags only; read-only) The third-party VAST tag you entered as the creative asset with the necessary Advertising Cloud tracking macros inserted, if applicable.

**Wmode:** (Some ad types) The window mode: *window*, *transparent*, or *opaque*.

### Teaser

*Mobile tap-to-play formats for DSP-served ads*

**Asset:** The teaser image or video asset:

* To select your own image, click **Choose File,** locate the file on your device or network, and then click **Upload Image**.

   The best practice is to use an image with the same dimensions as the ad unit.

* To select an image from the creative, click **Choose Thumbnail**.

Requirements for Static Image Teasers:

* Format: GIF, JPEG, PNG
* Image size: 300x250
* File size: 50KB or less
* Recommended: call to action, recognizable image, brand logo

Requirements for Video Teasers:

* File type: MOV, MP4  
* File Size: Less than 2MB
* Duration: 7-10sec
* Recommended: recognizable images, faces, quick cuts

### Overlays

*Interactive pre-roll and mobile interactive and tap-to-play formats for DSP-served ads*

The following settings apply to each overlay that you create or edit.

**Asset:** (Raw assets only) The overlay image asset. The file must be in single-frame GIF, JPG, or PNG format, and the maximum image size is less than 2MB. To upload the asset, click **Browse** and locate the file on your device or network, and then click **Upload**.

>[!TIP]
>
>See the [Best Practices for Designing Overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)

**Click URL:**  The URL on which the viewer will land when they click an overlay for your ad.

**X:** The X coordinate for the overlay. Select the overlay starting position, and then enter the number of pixels from the starting position (such as 10px From Center). The best practice is to use *From Center*, which prevents the overlay from moving around with different player sizes on publisher sites.

**Y:** The Y coordinate for the overlay. Select the overlay starting position, and then enter the number of pixels from the starting position (such as 10px from Top). The best practice is specify a coordinate *From Bottom* or *From Top,* depending the position in which you’d like the overlay to be displayed on the ad.

**Layer:** The layer in which the overlay will appear. The video and each overlay will be in separate layers.

* *2 through 5:* In front of the video but behind other overlays.

* *1:* In front of the video.

* *0:* In the same layer as the video. The video will shrink to fill the remaining space. Not recommended for Interactive Preroll.

* *-1:* Behind the video.

* *-2 through -5:* Behind the video but in front of other overlays.

* *Background:* Behind the video and other overlays. The overlay will scale to the full width and height of the video, and the aspect ratio won't be preserved.

### Endcap

Deprecated

### Pixel

All existing event tracking pixels for the placement are automatically attached. You can detach existing pixels and create new pixels as needed, based on your tracking needs.

The following settings apply to each pixel that you create or edit.

**Integration Event:** The event that triggers the pixel to fire. For this ad type, use pixels that fires on the *Impression* or *Click-through*.

**Pixel Type:** Whether the pixel is an *IMG URL* (1x1 pixel image file), *HTML*, or *JavaScript URL*.

**Pixel URL or Code:** The URL of the pixel image, in the appropriate format for the specified Pixel Type.

**Pixel Name:** The pixel name. Use a name that will help you easily identify the pixel.

**Pixel Provider:** The pixel provider: *None*, *Nielsen*, or *Comscore*.

### Sharing

Deprecated

>[!MORELIKETHIS]
>
>* [About Ad Management](ad-about.md)
>* [Create an Ad](ad-create.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
>* [Best Practices for Designing Overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)
