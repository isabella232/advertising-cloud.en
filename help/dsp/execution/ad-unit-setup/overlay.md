---
edit-last: 4
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Wed, 16 Jul 2014 08:18:28 +0000
dc-creator: hthomas@adobe.com
guid: https://education.tubemogul.com/?page_id=2272
isPermaLink: false
description: 
postId: 2272
postDate: 2014-07-16 00:18:28
postDateGmt: 2014-07-16 08:18:28
commentStatus: open
pingStatus: open
postName: overlay
status: publish
postParent: 1430
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Overlays {#overlays}

Overlays help with persistent branding throughout the video and can drive additional clicks. The overlay feature is available for:

* [Interactive Pre-roll](../../../dsp/planning/ad-formats/in-stream/interactive-pre-roll.md)
* [In-Display](../../../dsp/planning/ad-formats/in-display.md)
* [Facebook Unit](../../../dsp/planning/ad-formats/social.md)
* [Mobile Web CTP 300x250](mobile-setup/mobile-web-ctp.md)
* [Mobile App CTP 300x50](mobile-setup/mobile-app-ctp.md)
* [Mobile App Interactive](mobile-setup/mobile-app-interactive.md)

![overlay](assets/overlay.png)

* Asset:

    * URL field supports:

        * image (png, jpg, single-frame gif)
        * swfs (AS3, FP9, 30fps)
        * video (mp4, flv)

    * Upload button supports these file types: (<2MB)

        * image (png, jpg, single-frame gif)
        * swfs (AS3, FP9, 30fps)

    * Recommended Overlay Size:

        * Interactive Pre-roll: 350x60&#42;
        * In-display: 300x60
        * Full screen expandable: 728x90
        * Social: 470x70

* Click URL: landing page after viewer clicks on the overlay
* X: Recommended to "Center". It prevents the overlay from moving around due to different player sizes on publisher sites.
* Y:  "Bottom" or "Top" depending on what position you'd like the overlay to show up on the ad.
* Layer:

    * 1: In front of the video
    * 0: Same layer as the video; video will shrink to fill remaining space.  Not recommended for Interactive Preroll
    * -1: Behind the video
    * Background: Behind video and other overlays, will scale to full width & height, aspect ratio will not be preserved.

&#42;Interactive Preroll ads will vary in size based on the site, so we recommend overlays either be set to scale (by setting width and height to percentages) or be anchored only to one side of the ad with a ‘floating’ edge on the other side when scaling is not desired.  Scaling may distort text and details.  (See  [https://www.tubemogul.com/marketing/showcase/pre-roll-interactive.html](https://www.tubemogul.com/marketing/showcase/pre-roll-interactive.html) for examples.)

## Best Practices on Designing an Overlay

* When creating the overlay, it's recommended to review the video ad to ensure that any graphics, messaging or end-cap aren't covered by the design
* Animated overlays help to attract and engage viewers
* Using different colors than the video helps draw a viewer's eye to the overlay and call to action
* Overlay can display multiple buttons and/or call to actions, but keep the size of the overlay in mind (300x60 or 470x70)
* Overlays can be displayed horizontally or vertically
* The overlay shouldn't cover more than a 1/5 of the video (video player sizes can range from 720x480 to 400x300)

Examples can be found in our [Ad Gallery](https://gallery.tubemogul.com/overlay-animated.html).
If you have any additional questions, please reach out to [platform_support@tubemogul.com](mailto:platform_support@tubemogul.com).
