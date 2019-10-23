---
edit-last: 3
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
pubDate: Mon, 14 Jul 2014 20:04:34 +0000
dc-creator: hthomas@adobe.com
guid: http://education.tubemogul.com/?page_id=1828
isPermaLink: false
description: 
postId: 1828
postDate: 2014-07-14 12:04:34
postDateGmt: 2014-07-14 20:04:34
commentStatus: open
pingStatus: open
postName: companion-banner
status: publish
postParent: 1821
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Companion Banner {#companion-banner}

Companion banners are served alongside the pre-roll ad and can help reinforce brand and message association. TubeMogul serves these as value add and will be served around 30-40% of the time.

[ ![companion banner](assets/companion-banner.jpeg)](assets/companion-banner.jpeg)
&nbsp;   
**Upload Options:**
  
**For image assets:&nbsp;**

* **Option 1:** Upload my Own Asset

    * Image asset: jpeg, gif, img
    * Click URL: landing page or click redirect with 3rd party click tracking pixel
    * Use Option 2 if you want to track 3rd party companion banner impression as well. You'll need to create an iFrame using the template below.

* **Option 2:** Upload 3rd Party Tag- iFrame or script banner tag from one of our certified ad serving partners.

Example of an iFrame Template:   
<a href= "**INSERT CLICK&nbsp;TAG HERE**" target="_blank">   
<img src="**INSERT IMAGE FILE HERE**">   
</a> ${PIXELS} <img src="**INSERT IMPRESSION&nbsp;TRACKER HERE**">

* `<li>Copy the iFrame template to a text or word doc.</li>`  `<li>Replace the following in the iFrame: <br>  <ul>    <li>click_through_url= 3rd party click redirect with tracking pixel and landing page</li>    <li>banner_image= upload the asset to TubeMogul and take the url in the Asset field. Example above: http://playtime.tubemogul.com/ad_overlays/2325158_8488565.jpg</li>    <li>impression_pixel= 3rd party &nbsp;impression 1x1 tracker</li>   </ul> </li>`  `<li>Copy the filled out iFrame</li>`  `<li>Go back to the ad configurator, select the size, Upload via 3rd party and paste in the iFrame you just created.</li>`  `<li>Refresh and verify that the companion banner</li>`

**For Swf assets:&nbsp;**
For swf/flash files, please use the template below instead:   
<object type="application/x-shockwave-flash" data="**INSERT SWF FILE HERE**" width="300" height="250" id="tmContent_${RANDOM}" style="visibility: visible;">   
<param name="wmode" value="transparent"><param name="allowfullscreen" value="true"><param name="allowscriptaccess" value="always">   
<param name="flashvars" value="clickTag=**INSERT CLICK TAG HERE**">   
</object><script src="**INSERT IMPRESSION TRACKER HERE**"/>
  
&nbsp;   
**Sizes:&nbsp;**

* 300x250: most common and recommended on all pre-roll ads
* 300x60: recommended if running on YouTube sites
* 728x90: scarce

