---
title: Set up a Programmatic Guaranteed Deal
description: Learn how to set up a programmatic guaranteed (PG) deal you've negotiated with a publisher.
feature: Private Inventory, Deal IDs, Programmatic Guaranteed Deals
exl-id: 9e371606-5428-4635-9653-7dc43449e489
---
# Set up a Programmatic Guaranteed Deal

*[Supported supply side platforms only](programmatic-guaranteed-about.md)*

After you negotiate a programmatic guaranteed (PG) deal with a supported publisher, you can set up the deal within [!DNL DSP] either by using the deal ID inbox or by manually entering the deal details.

>[!NOTE]
>
> For PG deals, the publisher handles all budget pacing, budget capping, and targeting. All SSPs that allow PG through DSP confirm that the publisher can set up budget capping.
>
> Setting up programmatic guaranteed deals with publishers on FreeWheel requires extra permissions and steps. See "[Overview of Setting up Programmatic Guaranteed Deals in FreeWheel](freewheel-overview.md)" for more information.

## Set up a Programmatic Guaranteed Deal Using the Deal ID Inbox {#pg-setup-deal-id-inbox}

This is the preferred method for FreeWheel, Google Authorized Buyers, and Rubicon.

1. [Accept the deal](deal-id-inbox-accept.md).

1. After you save the deal, select the ads that will be used for the deal and create a programmatic guaranteed (PG) default placement, as prompted.

   Creating a default PG placement for the deal is mandatory to deliver 100% of your buy. This type of placement has no targeting so DSP can return a bid to every bid request from the publisher.
   
   * If you're accepting a single deal, you're automatically redirected to the PG default placement creation workflow.

     All Freewheel deals are proposed as a single deal.
   
   * If you're accepting a proposal with multiple PG deal IDs, then identify each PG default placement you need to create. Once you create all required placements, the continue button is enabled.

1. (Optional) Target the PG deal in additional, non-PG placements.

## Manually Set up a Programmatic Guaranteed Deal

Use this method for all other SSPs.

1. [Manually set up the deal ID details](deal-id-create.md).

1. After you save the deal, select the ads that will be used for the deal and create a PG default placement, as prompted.

   Creating a PG default placement for the deal is mandatory to deliver 100% of your buy. This type of placement has no targeting so DSP can return a bid to every bid request from the publisher.

1. (Optional) Target the PG deal in additional, non-PG placements.

>[!MORELIKETHIS]
>
>* [About Programmatic Guaranteed Deals](programmatic-guaranteed-about.md)
>* [Tips for Negotiating a Programmatic Guaranteed Deal](/help/dsp/inventory/programmatic-guaranteed-tips.md)
>* [Submit an Ad for a Programmatic Guaranteed Deal with Freewheel](freewheel-submit.md)
>* [Accept a Deal in the Deal ID Inbox](deal-id-inbox-accept.md)
>* [Manually Create Deal ID Details](deal-id-create.md)
>* [SSP Partners](ssp-partners.md)
>* [Overview of Inventory Features](inventory-overview.md)
