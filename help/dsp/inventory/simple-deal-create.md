---
title: Create a [!UICONTROL Simple Ad Serving] Deal
description: Learn how to create a tracking pixel for a [!UICONTROL Simple Ad Serving] deal.
feature: DSP Simple Ad Serving
exl-id:
---
# Create a [!UICONTROL Simple Ad Serving] Deal

1. In the main menu, click **[!UICONTROL Inventory] > [!UICONTROL Deals].**

1. Above the data table, click **[!UICONTROL Create]**, and then select **[!UICONTROL Simple Ad Serving]**.

1. Enter the [deal settings](simple-deal-settings.md):

   1. In the [!UICONTROL Select Ad Source] section, specify information about the publisher and ad type, and then click **[!UICONTROL Next]**.
   
   1. In the [!UICONTROL Select Ad(s)] section, specify the ad:

       1. Do either of the following:
      
         * For existing ads, select the ads.
        
         * For new ads, create the new [first-party ad](/help/dsp/campaign-management/ads/ad-create.md) or [third-party ad](/help/dsp/campaign-management/ads/ad-create-third-party).

       1. Click **[!UICONTROL Next]**.

   1. In the Feed Details, edit the feed details, and then click **[!UICONTROL Next]**.
   
       Advertising Cloud DSP automatically generates a placement, named "SAS Placement - &lt;*deal name*&gt;," for the ad. In the placement, the deal is automatically targeted in the [!UICONTROL Inventory Targets] section. All other targeting options are inapplicable.

1. Send the event-tracking pixels to the publisher for implementation in either of the following ways:

   * (Optional) From the [!UICONTROL Activate Tag with Publisher] screen, send the deal tag to the publisher.
   
     When you finish the previous steps, DSP generates an email message that you can send to the publisher. The message includes the deal details, a link from which to retrieve the deal tag, and an authorization code for the link.

     1. Review the deal details, and then do either of the following:
     
         * To paste the information into an email message in an email application on your device, click **[!UICONTROL Email & Done]** and select the email application. The [!UICONTROL CC:] field is prepopulated with an [!DNL Adobe] support address. You can then send the message to the appropriate contact for the publisher.

         * To copy the information to your clipboard, click **[!UICONTROL Copy Email].** You can then manually paste the contents into an email message and send it to the appropriate contact for the publisher. You must include a copy (CC:) to `publisher-support-global@adobe.com`. When you're finished copying the message, click **[!UICONTROL Email & Done]**.
    
      1. (If necessary) Follow up with the publisher to see if the tag includes the appropriate macros so that the tag will work with the publisher's ad server.

   * (Optional) Manually send the event-tracking pixels to the publisher:
   
     1. In the deal row within the [!UICONTROL Deals] view, click ![Options menu](/help/dsp/assets/options-menu.png) **> [!UICONTROL show pixel]**.
     
         The event pixels include a [!UICONTROL Clickthrough] pixel and an [!UICONTROL Impression] pixel. Video and audio ads also include event pixels by quartile completed (from [!UICONTROL 25% Complete] to [!UICONTROL 100% Complete]).

     1. Copy the event-tracking pixels and provide them to your publisher.

>[!MORELIKETHIS]
>
>* [About [!UICONTROL Simple Ad Serving]](simple-deal-about.md)
>* [[!UICONTROL Simple Ad Serving] Settings](simple-deal-settings.md)
>* [View Event-Tracking Pixels for a [!UICONTROL Simple Ad Serving] Deal](simple-deal-show-pixels.md)
