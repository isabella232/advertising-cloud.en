---
title: About the Deal ID Inbox
description: About the Deal ID Inbox
exl-id: 959ad1d4-4671-4967-9f73-ec5b0464d0cd
---
# About the Deal ID Inbox

DSP's Deal ID inbox allows you to quickly set up deals that Advertising Cloud DSP has imported from publishers through supply side platforms (SSPs) so you don't have to set up each deal manually. You can accept the guaranteed and non-guaranteed private inventory deals you've already negotiated with publishers on Google Authorized Buyers (formerly known as AdX), FreeWheel, and Rubicon, from the Deal ID Inbox.

>[!NOTE]
>
>Advertising Cloud DSP is the first DSP to integrate with the FreeWheel API.

In the deal ID inbox, you can see the details of the deal as your publisher sees them, speed up your deal setup, and avoid manual entry errors.

DSP automatically refreshes all deal details daily at 4:30 a.m. EST. It also refreshes all FreeWheel deals and updates existing deals from Google and Rubicon hourly. You can also manually refresh the deal details to populate new deals at any time.

<!-- MC: I'm not sure where I got the following. Is this currently true? -->
>[!NOTE]
>
>For programmatic guaranteed deals through Google Authorized Buyers, you must deliver on at least 90% of your budget or your account will lose access to Google deals in the deal ID inbox.

## Implementing the Deal ID Inbox

To receive your deals in the deal ID inbox, your SSP accounts must map your organization's DSP account to your SSP account. Contact your Adobe account manager for instructions.

>[!NOTE]
>
>DSP will share the organization's account names with the relevant SSPs.

During deal negotiations, tell the publisher to send the deal to your buyer instead of to the parent DSP account. The deal identifier may be a name or an ID, depending on the SSP.

## Actions You Can Take on Your Deals

* **Review deals** to verify that the SSP has sent the correct publisher, flight dates, CPM, and other deal details. If the publisher has made a mistake, contact them outside of DSP so they can correct and re-send the deal.

* **Accept deals** after reviewing, and they will no longer appear in the deal ID inbox. Accepted deals are listed in Inventory > Deals and are ready to target within advertisers’ placements.

* **Ignore deals** that aren't needed or are unsolicited. Ignored deals are moved to the Ignored Deals tab within the deal ID inbox, which serves as an archive. DSP doesn't alert SSPs and publishers when you ignore a deals.

* **Modify details for already-accepted deals** from Inventory > Deals (not in the deal ID inbox). Similarly, when publishers send changes to deals, advertisers are responsible for implementing those changes in Inventory > Deals because the deal ID inbox doesn't sync changes from the SSPs after deals are set up.

## What Types of Deals Can't Be Accepted?

When a deal listing doesn't include a ![Accept](/help/dsp/assets/accept.png) icon or an Accept button, you can't accept it from the deal ID inbox. Instead, you can [create the deal ID details manually](/help/dsp/inventory/deal-id-create.md).

You can't accept the following types of deals:

* Google deals that aren't in USD.

* Rubicon deals that aren't in USD

* FreeWheel deals that aren't in your account currency.

* Deals that have an end date before today.

* Old Rubicon deals that were labeled as "multiple media types."

The deal details include the reason the deal isn't available to accept.

>[!MORELIKETHIS]
>
>* [Accept a Deal in the Deal ID Inbox](deal-id-inbox-accept.md)
>* [Overview of Inventory Features](inventory-overview.md)
