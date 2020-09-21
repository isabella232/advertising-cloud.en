---
title: Manually Create Deal ID Details
description: Manually Create Deal ID Details
---
# Manually Create Deal ID Details

1. In the main menu, click **Inventory > Deals.**

1. Above the data table, click **Create**, and then select **Deal ID**.

1. Enter the [deal settings](deal-id-settings.md):

    1. In the **Deal ID basics** section, specify the deal details and the advertisers who can access the deal. For guaranteed deals, you must also specify the planned flight dates and the estimated of impressions, for tracking purposes only.

    1. (Administrator users only; optional) In the Technical section, edit the default settings as needed.

    1. Click **Save**.

1. (Guaranteed deals only) Select the ads that will be used for the deal and create a default programmatic guaranteed (PG) placement.

   Default PG placements ensure that your deal will always return a bid for every bid request. If you don't create a default PG placement, then any placements that target the deal won't place bids unless they're set up correctly. You should always create a default PG placement. In the Placements view, default PG placements have a Sub-type column value of "PG Default."
   
   You can optionally use the deal as an inventory target in additional placements but must set them up correctly to place bids.

    1. In the Ad & Campaign Selection settings, select the ads that will be used for the deal:

        1. Select the advertiser, campaign, and ad type.
        
        1. From the list of available ads, select the check box next to each ad that will be used for the deal.

        1. Click **Apply**.

    1. In the placement settings screen:
    
        1. Enter the placement name.
        
        1. (Optional) Edit the [placement settings](/help/dsp/campaign-management/placements/placement-settings.md), including overwriting the default bid, which is automatically populated with the CPM value from the deal; changing the date range; or attaching more ads.

           The deal is automatically targeted in the Inventory Targets section. All other targeting options are inapplicable.

        1. **Create placement**.

After you create the deal, you can use the deal as an inventory target for multiple placements.

>[!NOTE]
>
> You don't need to send the deal tag to the publisher for verification.

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
