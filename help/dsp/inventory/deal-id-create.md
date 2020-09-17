# Manually Create Deal ID Details {deal-id-create}

1. In the main menu, click **Inventory > Deals.**

1. Above the data table, click **Create**, and then select **Deal ID**.

1. Enter the [deal settings](deal-id-settings.md):

    1. In the **Deal ID basics** section, specify the deal details and the advertisers who can access the deal. For guaranteed deals, you must also specify the planned flight dates and the estimated of impressions, for tracking purposes only.

    1. (Administrator users only; optional) In the Technical section, edit the default settings as needed.

    1. Click **Save**.

1. (Guaranteed deals only) Select the ads that will be used for the deal and create a default placement.

   The deal isn't available as an inventory target in placement settings unless you create a default placement. You can override the default placement by using the deal as an inventory target in additional placements.  <!-- I don't see an option to create the default placement later if you exit the workflow without creating the placement. -- it has to be before you exit the workflow. -->

    1. In the Ad & Campaign Selection settings, select the ads that will be used for the deal:

        1. Select the advertiser, campaign, and ad type.
        
        1. From the list of available ads, select the check box next to each ad that will be used for the deal.

        1. Click **Apply**.

    1. In the placement settings screen:
    
        1. Enter the placement name.

           We recommend that you include “Default Placement" and "Guaranteed Feed” somewhere in the name to distinguish it from your other placements.
        
        1. (Optional) Edit the [placement settings](/help/dsp/campaign-management/placements\placement-settings.md), including overwriting the default bid, which is automatically populated with the CPM value from the deal; changing the date range; or attaching more ads.

           The deal is automatically targeted in the Inventory Targets section. All other targeting options are inapplicable.

        1. **Create placement**.

1. From the Feed Ad Tag screen, send the deal tag to the publisher for testing and verification.

   When you finish the previous steps, Advertising Cloud generates an email message that you can send to the publisher. The message includes the deal details, a link from which to retrieve the deal tag, an authorization code for the link, and contact information for reporting issues.

    1. In the Feed Ad Tag screen, review the deal details, and then do either of the following:
    
        * To paste the information into an email message in an email application on your device, click **Email** and select the email application. The CC: field is prepopulated with an Adobe support address (publisher-support-global@adobe.com). You can then send the message to the appropriate contact for the publisher.

        * To copy the information to your clipboard, click **Copy.** You can then manually paste the contents into an email message and send it to the appropriate contact for the publisher. You must include a copy (CC:) to publisher-support-global@adobe.com.

    1. Click **Finish**.
    
    1. (f necessary) Follow up with the publisher to see if the tag includes the appropriate macros so that the tag will work with the publisher's ad server.

After you create the feed, you can use the feed as an inventory target for multiple placements.

>[!TIP]
>
>* In the Inventory > Deals view, the Pacing & Budget column will show how the deal is pacing to the specified flight date and impression goal.
>
>* If delivery is under- or over-pacing, contact your publisher to adjust how much volume it is sending through the deal.

>[!MORELIKETHIS]
>
<!-- >* [About Private Inventory](private-inventory-about.md) -->
>* [Manual Deal ID Settings](deal-id-settings.md)
>* [Set up a Programmatic Guaranteed Deal](programmatic-guaranteed-setup.md)
>* [About Programmatic Guaranteed Deals](programmatic-guaranteed-about.md)
