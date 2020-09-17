# Manual Deal ID Settings {#deal-id-settings}

## Deal ID basics

### [Deal Details and Billing Method]

**Deal name:**  The name you will use to identify your Deal ID in Advertising Cloud DSP. Enter a name or select **Auto-name** to let Advertising Cloud generate a name based on the deal details.

Example of an auto generated name: *DEAL_ID* - Deal ID - Guaranteed Fixed - USD - 5 - 24Kitchen - Private

**External deal ID:** (Read-only for existing deals) The ID used by your publisher and the SSP to identify this deal.

**Publisher:** (Read-only for existing deals) The name of the publisher that is selling this inventory.

**SSP:** (Read-only for existing deals) The supply side platform (SSP) through which this deal will run.

**Media type:** (Read-only for existing deals) The type of media that will bought through this deal:  *Desktop video*, *Mobile video*, *Connected TV*, *Display*, or *Audio*. The options vary by SSP.

**Deal type:** (Read-only for existing deals) The deal commitment and pricing structure:

* *Non guaranteed (floor):* You and the publisher haven't committed to a fixed number of impression deliveries. The deal specifies the minimum price for the inventory, although the CPM may fluctuate and increase depending on market conditions.

* *Non guaranteed (fixed):* You and the publisher haven't committed to a fixed number of impression deliveries. Pricing is at a negotiated fixed rate.

* *Guaranteed (fixed):*  You and the publisher have agreed on a pre-defined number of impressions, targeting, flight dates, and fixed price, so you’ll buy any or all impressions that come through the deal. 

>[!NOTE]
>
>Guaranteed deals require flight dates and a specified number of impressions in the Tracking section. You'll also need to create a default placement for the deal, although you can optionally use the deal for other placements instead.

**CPM:** The negotiated cost per thousand impressions (CPM) and the currency for the deal.

Google and Rubicon accept deals only in USD. For FreeWheel, you can optionally select the currency for the DSP account. <!-- FreeWheel is the only SSP with non-US currencies. -->

**Billing method:** (Read-only for existing deals) All deal IDs are *Adobe financed and invoiced*. Advertising Cloud will pay all available media vendors based on usage, manage discrepancies with the vendors, and send one consolidated invoice to the account. This option incurs additional fees as outlined in [the account's rate card](/help/dsp/admin/rate-card-view.md).

### Advertisers

**Account email:** (Optional) The email address for the user account that can access the deal.

**Advertisers that can access this deal:** The specific advertisers in the account who can access this deal.

>[!NOTE]
>
>Administrator users can give access to advertisers in multiple accounts.

### Tracking

>[!TIP]
>
>* In the Inventory > Deals view, the Pacing & Budget column will show how the deal is pacing to the specified flight date and impression goal.

>* If delivery is under- or over-pacing, contact your publisher to adjust how much volume it is sending through the deal.

**Flight Dates:** (Optional for non-guaranteed deals) The start and end dates for traffic using this deal. These date are for tracking purposes only and don't impact ad delivery.

**Impressions:** (Optional for non-guaranteed deals) The estimated number of impressions you expect to run using this deal. This value is tracking purposes only; the publisher controls ad delivery.

## Technical (Enabled for administrator users only)

**Enable fraud protection:** (Optional) Enables site safety protection for this deal. By default, this option is disabled.

Disable this option to serve ads in embedded players, whose URLs may not be included in your placement site lists.

**100% mobile and CTV viewability:** (Optional) Makes impressions on mobile apps and connected TV apps 100% viewable and 100% measurable when the video reaches 25% completion. <!-- verify this -->

>[!IMPORTANT]
>
>Enable this option only for inventory that Advertising Cloud has confirmed as viewable.

**Pixel timeout (minutes):** (New deals only) The number of minutes after an auction win during which DSP will record all impression pixel fires as impressions. All impressions recorded within the pixel timeout duration will be billed to the account. The default for all media types is 180 minutes. If necessary, enter a new pixel timeout, or select **Exempt from pixel timeout** to ignore the pixel timeout.

>[!IMPORTANT]
>
>When a deal is exempt from the pixel timeout, all impressions recorded at any time after the auction is won, even years later, are billed to the account. Use the exempt option with caution.

>[!MORELIKETHIS]
>
>* [About Private Inventory](private-inventory-about.md)
>* [Create Manual Deal ID Details](deal-id-create.md)
