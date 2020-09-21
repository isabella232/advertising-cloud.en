---
title: Companion Banner
description: Companion Banner
---

# Companion Banner

Companion banners are served alongside pre-roll ads or (with some publishers) audio ads and can help reinforce brand and message association.

>[!NOTE]
>
> Not all publishers allow companion banners. The publishers who do allow companion banners don't guarantee companion banner impressions.
> Companion banners from third-party ad tags may not always available for preview.

## Upload Options
  
### Image assets

* Option 1: Upload my Own Asset

  * Image asset: jpeg, gif, img
  * Click URL: landing page or click redirect with 3rd party click tracking pixel
  * Use Option 2 if you want to track 3rd party companion banner impression as well. You'll need to create an iFrame using the template below.

* Option 2: Upload 3rd Party Tag- iFrame or script banner tag from one of our certified ad serving partners

Example of an iFrame Template:

```
<a href= "<INSERT CLICK TAG HERE>" target="_blank">   
<img src="<INSERT IMAGE FILE HERE>">   
</a> ${PIXELS} <img src="<INSERT IMPRESSION TRACKER HERE>">
```

* Copy the iFrame template to a text or word doc.
* Replace the following in the iFrame:

  * click_through_url= 3rd party click redirect with tracking pixel and landing page
  * banner_image= upload the asset and take the url in the Asset field. Example above: `http://playtime.tubemogul.com/ad_overlays/2325158_8488565.jpg`  <!-- need to create a new example on https://advertising.adobe.com -->
  * impression_pixel= 3rd party  impression 1x1 tracker

* Copy the filled out iFrame
* Go back to the ad configurator, select the size, Upload via 3rd party and paste in the iFrame you just created.
* Refresh and verify that the companion banner

### SWF assets

For swf/flash files, use the following template:

```
<object type="application/x-shockwave-flash" data="<INSERT SWF FILE HERE>" width="300" height="250" id="tmContent_${RANDOM}" style="visibility: visible;">   
<param name="wmode" value="transparent"><param name="allowfullscreen" value="true"><param name="allowscriptaccess" value="always">   
<param name="flashvars" value="clickTag=<INSERT CLICK TAG HERE>">   
</object><script src="<INSERT IMPRESSION TRACKER HERE>"/>
```

## Sizes

* 300x250: most common and recommended on all pre-roll ads
* 300x60: recommended if running on YouTube sites
* 728x90: scarce
