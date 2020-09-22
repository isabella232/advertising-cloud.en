---
title: Smart Ad Serving Deal Settings
description: Smart Ad Serving Deal Settings
---

# Smart Ad Serving Deal Settings

<!-- ## Screen 1 -->

## Feed Name

The deal name. Enter a name, or select *Autogenerate Name* to let Advertising Cloud generate a name based on the deal details.

Example of an auto generated name: RTBDB – CNN via appnexus – jdoe – USD – $20.00 – :30 – PMP

## Billing Option

How to be billed for usage:

* *Adobe Financed and Invoiced:* Advertising Cloud will pay all available media vendors based on usage, manage discrepancies with the vendors, and send one consolidated invoice to the account. This option incurs additional fees as outlined in the account's rate card<!-- [the account's rate card](/help/dsp/admin/rate-card-view.md) -->.
    
  This option is available only when it's activated. Contact your Adobe account manager to activate it.
    
* *Adobe Managed and Supplier Invoiced:* The Adobe Client Services team will provide turnkey execution of your deal, and you will receive the following bills:
    
    * A media bill sent directly from the media vendor (typically the publisher or a supply side platform (SSP)).
        
    * A platform fees invoice from Advertising Cloud, according to the fees outlined in the account's rate card<!-- [the account's rate card](/help/dsp/admin/rate-card-view.md)-->.

## Feed Access

The specific advertisers in the account who can access this deal.

<!-- ## Screen 2 -->

## Publisher Settings

**Publisher/Media Owner:** The name of the publisher that is selling this inventory. Search for a publisher by entering at least the first two characters in the name. To add a publisher that isn't listed, contact your Adobe account manager.

**Billing Entity/Media Vendor:** The media vendor that will send the bill.

**Publisher Maximum Ad Length:** The maximum duration of the ads accepted by the selected publisher. The default is 30 seconds.

**Publisher Maximum Ad Length:**  The minimum duration of the ads accepted by the selected publisher. The default is 10 seconds.

## Inventory Types

The media type and ad specification for this deal: <!-- The available ad specs seem to be the same across all publishers, but verify. -->

* *Desktop Video:* Available ad specifications include *VAST Only*, *VAST and VPAID JS*, or *VAST and VPAID Flash*.
    
* *Mobile Video:* Available ad specifications include *VAST Only* or *VAST and VPAID JS*.
    
* *Connected TV Video:* Available ad specifications include *VAST Only*.
    
* *Audio:* Available ad specifications include *VAST Only*.

## Economics

**Fill Type:** The deal commitment:

* *Guaranteed* buy: You and the publisher have agreed on a pre-defined number of impressions, targeting, and flight dates, so you’ll buy any or all impressions that come through the deal. 
    
* *Non-Guaranteed* buy: You and the publisher haven't committed to a fixed number of impression deliveries.

**Contracted CPM:** The negotiated cost per thousand impressions (CPM) and the currency for the deal.

All users can select USD, or, if the SSP supports additional currencies, the currency for the DSP account.

**`[CPM Pricing Structure`]:** (Non-Guaranteed buys only) Whether the pricing structure is for a:

* *Fixed CPM:* The negotiated fixed rate.
* *Floor CPM:* The minimum price for the inventory, although the CPM may fluctuate and increase depending on market conditions.

## Flighting

>[!TIP]
>
>* In the Inventory > Deals view, the Pacing & Budget column will show how the deal is pacing to the specified flight date and impression goal.

>* If delivery is under- or over-pacing, contact your publisher to adjust how much volume it is sending through the deal.

**Flight Dates:** (Optional for non-guaranteed deals) The start and end dates for traffic using this deal. These date are for tracking purposes only and don't impact ad delivery.

**Target Impressions:**  (Optional for non-guaranteed deals) The estimated number of impressions you expect to run using this deal. This value is tracking purposes only; the publisher controls ad delivery.

## Attribute Tags

(Optional) Any existing attribute tags to add to the deal record so that campaign managers can easily locate the deal when they create placements.

>[!MORELIKETHIS]
>
>* [About Private Inventory](private-inventory-about.md)
>* [Create a Smart Ad Serving Deal](smart-deal-create.md) <!-- probably will rename title and filename -->
