---
title: Create a Simple Ad Serving Deal
description: Create a Simple Ad Serving Deal
---

# Create a Simple Ad Serving Deal

1. In the main menu, click **Inventory > Deals.**

1. Above the data table, click **Create**, and then select **Simple Ad Serving**.

1. Enter the [deal settings](simple-deal-settings.md):

    1. In the Select Ad Source section, specify the XXX, and then click **Next**.

    1. In the Select Ad(s) section, specify the ad:

        1. Do either of the following:
    
            * For existing ads, select the ads.
        
            * For new ads, create the new [first-party ad](/help/dsp/campaign-management/ads/ad-create.md) or [third-party ad]((/help/dsp/campaign-management/ads/ad-create-third-party).

        1. Click **Next**.

    1. In the Feed Details, edit the feed details, and then click **Next**.

   Advertising Cloud automatically generates a placement, named "SAS Placement - &lt;*deal name*&gt;," for the ad. In the placement, the deal is automatically targeted in the Inventory Targets section. All other targeting options are inapplicable. <!-- This is supposed to be a default placement, since this is programmatic guaranteed, but I don't see the deal listed in placement settings, so I'm second-guessing that. How do I add it to another placement? -->

1. From the Activate Tag with Publisher screen, send the deal tag to the publisher for testing and verification.

   When you finish the previous steps, Advertising Cloud generates an email message that you can send to the publisher. The message includes the deal details, a link from which to retrieve the deal tag, and an authorization code for the link.

    1. Review the deal details, and then do either of the following:
    
        * To paste the information into an email message in an email application on your device, click **Email & Done** and select the email application. The CC: field is prepopulated with an Adobe support address (publisher-support-global@adobe.com). You can then send the message to the appropriate contact for the publisher.

        * To copy the information to your clipboard, click **Copy Email.** You can then manually paste the contents into an email message and send it to the appropriate contact for the publisher. You must include a copy (CC:) to publisher-support-global@adobe.com. When you're finished copying the message, click **Email & Done**.
    
    1. (If necessary) Follow up with the publisher to see if the tag includes the appropriate macros so that the tag will work with the publisher's ad server.

>[!TIP]
>
>* In the Inventory > Deals view, the Pacing & Budget column will show how the deal is pacing to the specified flight date and impression goal.
>
>* If delivery is under- or over-pacing, contact your publisher to adjust how much volume it is sending through the deal.

>[!MORELIKETHIS]
>
>* [About Private Inventory](private-inventory-about.md)
>* [Simple Ad Serving Settings](simple-deal-settings.md)
