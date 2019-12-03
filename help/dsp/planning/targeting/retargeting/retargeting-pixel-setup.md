---
edit-last: 4
wp-page-template: page-left-sidebar.php
rawhtml-settings: 0,0,0,0
ldc-disable: 0
ldc-disable-comm: 0
pubDate: Fri, 04 Jul 2014 16:05:40 +0000
dc-creator: hchang@adobe.com
guid: https://education.tubemogul.com/userguide/?page_id=1502
isPermaLink: false
description: 
postId: 1502
postDate: 2014-07-04 08:05:40
postDateGmt: 2014-07-04 16:05:40
commentStatus: open
pingStatus: open
postName: retargeting-pixel-setup
status: publish
postParent: 1500
menuOrder: 0
postType: page
postPassword: 
isSticky: 0
---

# Retargeting Pixel Setup {#retargeting-pixel-setup}

1.In the main menu, select **DSP > Tools > Segments**.

1. Click **New Custom Segment**, enter the segment name, and then click **Save and Close**.

   Use a segment name that clearly states the type of cookie pool you are collecting (such as Homepage Visitors- Site X).
  
1. In the Options column, click the gear icon on the right side and select **get pixel**.

   Use the HTML tag if you are placing it on a website, and use the Flash tag if you are attaching it to an ad.
  
   ![segment](assets/segment-300x169.png)
  
1. Use a debugging tool such as Charles or Fiddler to verify that the pixel is firing correctly.
  
1. Check the Segments Manager periodically to confirm the segment size increases.
