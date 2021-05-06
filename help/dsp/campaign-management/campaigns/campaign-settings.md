---
title: Campaign Settings
description: See descriptions of the available campaign settings.
feature: campaign management, campaigns
exl-id: ff2e22ff-8073-4532-884b-36e0c1f22641
---
# Campaign Settings

## Basic Campaign Details

**Name:** The campaign name.

**Advertiser:** (Read-only for existing campaigns) The applicable advertiser (brand). Select an existing advertiser or create a new one.

**Advertiser URL:** The advertiser’s official page. This field speeds your ad approval process with inventory partners.

**Timezone:** (Read-only for existing campaigns) The timezone for reporting and bidding.

**Customer PO:** (Optional) A customer purchase order for the insertion order/purchase order.

**Campaign Dates:** The campaign start and end dates.

## Campaign Goals

**Margin Management:** Whether to manage margins for the campaign: *Yes* or *No* (the default).

When you choose *Yes,* specify the margin type and amount:

* **Margin Type:** The type of margin. You can't change the margin type once you enable margin management and save the campaign.
   
   * *Fixed:* (the default) Allows Advertising Cloud DSP to auto-calculate and cap spend based on a fixed margin percentage of the Gross Budget.
   
   * *Dynamic:* Allows you to manage margins down to the placement level by specifying a separate Budget Reserve % and Gross Budget for each package and placement in the campaign. Advertising Cloud DSP optimizes based on the financial efficiency of each placement, without guaranteeing a specific margin. Use this for insertion orders that consist of multiple line items for which you've agreed to deliver a fixed amount of units or unit types at a fixed rate.

* **Fixed Margin %:** (Campaigns with fixed margins only) The default markup for each insertion order <!-- impression? -->, as a percentage. This amount is deducted from the Gross Budget to define the net campaign budget.

* **Budget Reserve %:** (Campaigns with fixed margins only; optional) Reserves a specified percentage of the gross budget as a safeguard. This amount is deducted from the Gross Budget to define the net campaign budget.

**Gross Budget:** (Campaigns with margin management only) The gross campaign budget, before the specified marginal adjustments are applied.

You can optionally add an additional daily, weekly, or monthly gross budget:

1. Click **Add an additional Gross Budget**.

1. Enter the **Gross Budget** and select the budget interval: *Daily,* *Weekly,* or *Monthly*.

 The total net budget, which is the spending cap for the campaign, is automatically calculated based on the margin settings and is indicated below this value.

**Budget:** (Campaigns without margin management) The overall campaign budget.

**Estimated Tax Withholding:** Withholds a percentage of total spend across ad fees, ad serving fees, and/or data fees at the account level for country or local taxes. Rates are estimates for budgeting and pacing purposes, so invoiced tax rates may vary.

To estimate taxes to withhold:

1. Click **Update rates here**.

1. Specify the *Estimated tax rate**, as a percentage.

1. Select the check box next to each fee type for which to withhold taxes. The fee types include:

   * *Include estimated tax - ads fee:* Applies to all Advertising Cloud DSP media spend, including taxes on campaign management fees.
   
   * *Include estimated tax - ad serving fee:* Applies to all spend on Advertising Cloud DSP except for media and data. It excludes taxes for campaign management fees
   
   * *Include estimated tax - data fee:* Applies to all data spend on Advertising Cloud DSP.

1. Click **Submit**.

>[!NOTE]
>
>* In the U.S., states may vary in their inclusion of tax fees across ads, ad serving, and data. For organizations in other countries, include all three categories of tax fees to account for VAT.
>
>* You can also configure these values in the account's fee settings.<!--[fee settings](/help/dsp/admin/tax-withholdings.md). -->

**Cross Device Level:** (Read-only for existing campaigns created since 22 June 2020; not available for campaigns created before 22 June 2020) The level at which Advertising Cloud will target ads and apply frequency caps: *Same Device* to target a device or *People* to target a person across all of their known devices.

**Device Graph:** (Read-only for existing campaigns; campaigns with people-based cross-device targeting only) The device graph to use for cross-device targeting and frequency management:

* *LiveRamp - U.S. only:* Available to all advertisers for cross-device targeting at $0.35 CPM for impressions that are delivered by using the LiveRamp device graph (that is, for devices not found within the targeted audience segments). You can set up cross-device targeting at the placement level.

    This option is also available to all advertisers, without any fees, for frequency management and attribution measurement.

* *Adobe Co-op U.S. and Canada only:* Available only to Adobe Experience Cloud Device Co-op participants at no extra fee.

>[!TIP]
>
>If the advertiser also uses cross-device attribution, then the best practice is to use the same device graph settings for targeting and frequency management as those that are specified in the advertiser's cross-device attribution settings. If you select a different device graph for this campaign, then reporting discrepancies may occur.

**Frequency Cap:** (Optional) The number of times a unique device or person (depending on the specified Cross Device Level) will be served ads from the campaign. Options include *Unlimited* or a specific amount per day, week, or month.

>[!NOTE]
>
> You can set frequency caps at the campaign, package, and placement levels. DSP will respect the strictest frequency cap in the campaign hierarchy.

**Packages:** The [packages](/help/dsp/campaign-management/packages/package-about.md) to include in the campaign. Select existing packages and/or create packages to include. If you create packages, see descriptions about the [package settings](/help/dsp/campaign-management/packages/package-settings.md) for more information.

## Campaign Measurement

>[!NOTE]
>
>The following settings enable only measurement and reporting capabilities. Performance optimization is executed only at the package and placement level.

### 3rd Party Metrics

#### Viewability, Fraud, & Brand Safety

**IAS:** (Optional) Enables IAS measurement and reporting of viewability, fraud, brand safety, and audience verification, using the specified settings. Additional fees apply.

* **Measure On:** The inventory on which to measure: *Display and VPAID video inventory* (the default) or *Display, VPAID & VAST video inventory*.

   >[!NOTE]
   >
   >Video viewability is measurable on VPAID inventory only.

* **IAS Account ID (AnID):** (Advertisers with their own IAS accounts; optional) The organization's IAS account ID, which IAS will bill directly for usage.

* **IAS Team ID:** (Advertisers with their own IAS accounts; optional) The team ID for the organization's IAS account, which IAS will bill directly for usage. <!-- verify -->

**MOAT:** (Optional) Enables MOAT measurement and reporting of viewability, fraud, brand safety, and audience verification. Additional fees apply.

#### Audience Verification

**Nielsen:** (Optional) Enables Nielsen measurement and reporting of audience verification, using the specified settings. Additional fees apply.

* **Target Gender:** The gender to target: *Both* (the default), *Male*, or *Female*

* **Target Age:** The age range to target. Use the left and right sliders to reduce the range as needed.

* **Target Country:** (Optional) A country to target. Nielsen will measure impressions served in supported countries only.

**comScore vCE:** (Optional) Enables Comscore validated Campaign Essentials (vCE) measurement and reporting of audience verification, using the specified settings. Additional fees apply.

* **Target Gender:** The gender to target: *Both* (the default), *Male*, or *Female*

* **Target Age:** The age range to target. Use the left and right sliders to reduce the range as needed.

* **Target Country:** (Optional) A country to target. Comscore will measure impressions served in supported countries only.

### 1st Party Metrics

**Viewability sensitivity:** Enables first-party measurement and reporting of viewability using the IAB Open Video Viewability (OpenVV) technology, based on the specified sensitivity level:

* *Standard (50% of ad in view for two consecutive seconds)*

* *Strict (100% of ad in view and audio on for 50% duration)*

>[!MORELIKETHIS]
>
>* [About Campaign Management](campaign-about.md)
>* [Create a Campaign](campaign-create.md)
>* [Edit a Campaign](campaign-edit.md)
