---
title: Using Roku Inventory
description: Learn about DSP's partnership with Roku, including inventory options, approved third-party tracking vendors, and best practices for Roku-specific placements. 
feature: inventory, connected TV
exl-id: 0cd42782-f006-4aa8-b879-322f86cfac4b
---
# Using Roku Inventory

Advertising Cloud DSP provides unique features for advertising on Roku.

## The Advertising Cloud DSP and Roku Partnership

Roku and Advertising Cloud DSP have a unique partnership that matches your DSP audiences to Roku IDs for 1:1 deterministic audience targeting on Roku inventory.

Outside of Roku’s own DSP (OneView), Advertising Cloud DSP has sole access to these targeting capabilities. Advertising Cloud DSP is also the only DSP with permission to measure Roku supply next to all other connected TV (CTV) inventory. Because Roku doesn't share all of the standard RTB and impression pixel signals, no other DSP can target or measure across Roku-sold CTV supply.

## Roku Inventory Options

You can either a) set up private deal IDs directly with Roku and then enter the deal ID data into DSP or b) visit the On Demand Gallery to subscribe to Roku profiles:

>[!NOTE]
>
>Roku inventory isn't available in open marketplaces and exchanges.

* For your private deals, you'll [set up information about the deal IDs in DSP](/help/dsp/inventory/deal-id-create.md) and then target “Roku Network – Audience” and “The Roku Channel – Audience” within Roku placements.<!-- Or do you target the deal ID?? I see those strings for Roku On Demand inventory. Clarify if all Roku private deals will show up as one or the other of these in Roku Private inventory in Roku placement settings. -->

* You can [subscribe to the following Roku inventory within the On Demand Gallery](/help/dsp/inventory/on-demand-inventory-subscribe.md), and then target any of the approved deals within Roku placements:

    * “Roku Network – Audience” for inventory across the Roku ecosystem with premium content partners, such as The CW, ABC, and ESPN.
    * “The Roku Channel – Audience” for Roku’s owned-and-operated (O&O) app content.

### Advantages of Customizing Private Marketplaces with Roku

Private deals allow you to customize the deal parameters according to your needs.

* **Negotiated pricing:** Work with the Roku sales team to negotiate and structure a deal that meet your campaign needs.

* **Scale Priority:** Private marketplaces (PMPs) receive higher priority than always-on deals (such as On Demand deals).

* **Frequency Management:** Roku's default frequency cap is one (1) ad per 30 minutes per user, but you can customize the cap by hour, day, week, month, or entire flight period.<!-- Within the DSP placement settings? NO - you negotiate this with Roku, but Christine to confirm with Amanda whether you should be able to edit this in placement. -->

* **Roku Data Targeting:** Roku audiences are built from Roku device and TV signals, data tracked by The Roku Channel (such as TV genre affinity, streaming TV behavior, and cable subscription status), and additional data from Roku's customer relationship management (CRM) system.

* **Roku Content Targeting:** Private deals can target apps by genre, application of app blocklist, seasonal and tentpole events, and shows within The Roku Channel only.

## Roku Placements

In DSP campaigns, you'll [create Roku-specific placements](/help/dsp/campaign-management/placements/placement-create.md) using the placement type "Connected TV (Roku)." You'll include Roku placements in Roku-specific packages with defined goals.

Each Roku placement must target at least one Roku deal or source. To leverage DSP’s unique audience matching with Roku, include one or more one audience segments that can be matched against Roku’s (opted-in) deterministic dataset.

### Roku-Approved Third-Party Tracking Vendors

Roku placements can include third-party event pixels and conversion pixels from the following vendors:  Acxiom, comScore, Data Plus Math, Experian, Factual, Kantar, Marketing Evolution, Neustar, Nielsen, Nielsen Catalina Solutions, NinthDecimal, Oracle, Placed, Polk, and Research Now.

### Best Practices by Placement Strategy

 The following are the recommended practices for Roku-specific placements.

To maximize incremental reach:

* Suppress exposed audiences on Roku O&O by excluding audiences you've already reached using The Roku Channel.

* Suppress exposed audiences on All Roku by excluding audiences you've already reached across the Roku platform.

For the fastest setup:

* Target existing, always-on deals for The Roku Channel in [On Demand Inventory](/help/dsp/inventory/on-demand-inventory-subscribe.md) to quickly access Roku owned-and-operated inventory.
* Target existing, always-on deals for Roku Network in [On Demand Inventory](/help/dsp/inventory/on-demand-inventory-subscribe.md) to quickly achieve scale across the Roku platform.

To maximum scale:

* Customize a Roku private marketplace for prioritized access to Roku supply at a negotiated price.

>[!MORELIKETHIS]
>
>* [Manually Create Deal ID Details](/help/dsp/inventory/deal-id-create.md)
> * [Subscribe and Request Access to On Demand Premium Inventory Deals](/help/dsp/inventory/on-demand-inventory-subscribe.md)
>* [Create a Placement](/help/dsp/campaign-management/placements/placement-create.md)
