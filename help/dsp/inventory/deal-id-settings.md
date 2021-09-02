---
title: Manual Deal ID Settings
description: See descriptions of the settings for manually-entered Deal IDs.
feature: Private Inventory, Deal IDs
exl-id: 0cd5e9e8-2b13-4b1e-a2e0-b8b492f75acf
---
# Manual Deal ID Settings

<!-- Can't use !UICONTROL and !DNL tags in HTML table -- change to Markdown and add the tags. -->

<!-- 
<table>
    <tr>
       <td><p><b>Section</b></p></td>
       <td><p><b>Parameter</b></p></td>
       <td><p><b>Description</b></p></td>
       <td><p><b>Required</b></p></td>
       <td><p><b>Editable</b></p></td>
    </tr>
    <tr>
       <td><p>[Deal Details]</p></td>
       <td><p>Deal name</p></td>
       <td><p>The name to identify your Deal ID in Advertising Cloud DSP. Enter a name or select <b>Auto-name</b> to let Advertising Cloud generate a name based on the deal details.</p>
       <p>Example of an auto generated name: *DEAL_ID* - Deal ID - Guaranteed Fixed - USD - 5 - 24Kitchen - Private</p></td>
       <td><p>Yes</p></td>
       <td><p>Yes</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>External deal ID</p></td>
       <td><p>The ID used by your publisher and the SSP to identify this deal.</p></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>Publisher</p></td>
       <td><p>The name of the publisher that is selling this inventory.</p></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>SSP</p></td>
       <td><p>The supply side platform (SSP) through which this deal will run.</p></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>Media type</p></td>
       <td><p>The type of media that will bought through this deal: <i>Desktop video</i>, <i>Mobile video</i>, <i>Connected TV</i>, <i>Display</i>, or <i>Audio</i>. The options vary by SSP.</p></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>Deal type</p></td>
       <td><p>The deal commitment and pricing structure:</p>
       <ul>
          <li><p><i>Non guaranteed (floor)</i>: You and the publisher haven't committed to a fixed number of impression deliveries. The deal specifies the minimum price for the inventory, although the CPM may fluctuate and increase depending on market conditions.</p></li>
          <li><p><i>Non guaranteed (fixed)</i>: You and the publisher haven't committed to a fixed number of impression deliveries. Pricing is at a negotiated fixed rate.</p></li>
          <li><p><i>Guaranteed (fixed)</i>: You and the publisher have agreed on a pre-defined number of impressions, targeting, flight dates, and fixed price.</p>
          <p><b>Note:</b> Guaranteed deals require flight dates and a specified number of impressions in the Tracking section. You'll also need to create a default programmatic guaranteed (PG) placement for the deal, and you can optionally use the deal for other placements instead.</p></li>
       </ul></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>CPM</p></td>
       <td><p>The negotiated cost per thousand impressions (CPM).</p></td>
       <td><p>Yes</p></td>
       <td><p>Yes</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>[Currency]</p></td>
       <td><p>The currency for the deal.</p>
       <p>All SSPs accept deals in USD. When the SSP accepts the currency for your [!DNL DSP] account, that currency is also available.</p></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>Billing method</p></td>
       <td><p>All deal IDs are <i>Adobe financed and invoiced</i>. Advertising Cloud will pay all available media vendors based on usage, manage discrepancies with the vendors, and send one consolidated invoice to the account. This option incurs additional fees as outlined in the account's rate card.</p></td>
       <td><p>Yes</p></td>
       <td><p>No</p></td>
    </tr>
    <tr>
       <td><p>Advertisers</p></td>
       <td><p>Account email</p></td>
       <td><p>The email address for the user account that can access the deal.</p></td>
       <td><p>No</p></td>
       <td><p>Yes</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>Advertisers that can access this deal</p></td>
       <td><p>The specific advertisers in the account who can access this deal.</p>
       <p><b>Note:</b> You can share the deal with advertisers in additional accounts from the Deals view. In the deal row, click <img src="/help/dsp/assets/edit.png">, click <b>share</b>, and then share the deal with an email address.</p></td>
       <td><p>Yes</p></td>
       <td><p>Yes</p></td>
    </tr>
    <tr>
       <td><p>Tracking</p></td>
       <td><p>Flight Dates</p></td>
       <td><p>The start and end dates for traffic using this deal. These date are for tracking purposes only and don't impact ad delivery.</p>
       <p><b>Tip:</b> In the Inventory &gt; Deals view, the Pacing &amp; Budget column will show how the deal is pacing to the specified flight date and impression goal. If delivery is under- or over-pacing, contact your publisher to adjust how much volume it is sending through the deal.</p></td>
       <td><p>Guaranteed deals: Yes</p>
       <p>Non-guaranteed deals: No</p></td>
       <td><p>Yes</p></td>
    </tr>
    <tr>
       <td><p>&#160;</p></td>
       <td><p>Impressions</p></td>
       <td><p>(Optional for non-guaranteed deals) The estimated number of impressions you expect to run using this deal. This value is tracking purposes only; the publisher controls ad delivery.</p></td>
       <td><p>Guaranteed deals: Yes</p>
       <p>Non-guaranteed deals: No</p></td>
       <td><p>Yes</p></td>
    </tr>
</table>
 -->

| Section | Parameter | Description | Required | Editable |
|---------|-----------|-------------|----------|----------|
| [Deal Details] | [!UICONTROL Deal nam]e | The name to identify your [!UICONTROL Deal ID] in Advertising Cloud DSP. Enter a name or select [!UICONTROL Auto-name] to let Advertising Cloud generate a name based on the deal details.<br><br>Example of an auto generated name: [!DNL *DEAL_ID* - Deal ID - Guaranteed Fixed - USD - 5 - 24Kitchen - Private] | Yes | Yes |
| | [!UICONTROL External deal ID] | The ID used by your publisher and the SSP to identify this deal. | Yes | No |
| | [!UICONTROL Publisher] | The name of the publisher that is selling this inventory.| Yes | No |
| | [!UICONTROL SSP] | The supply side platform (SSP) through which this deal will run. | Yes | No |
| | [!UICONTROL Media type] | The type of media that will bought through this deal: [!UICONTROL Desktop video], [!UICONTROL Mobile video], [!UICONTROL Connected TV], [!UICONTROL Display], or [!UICONTROL Audio]. The options vary by SSP. | Yes  | No |
| | [!UICONTROL Deal type] | The deal commitment and pricing structure:<br><ul><li>[!UICONTROL Non guaranteed (floor)]: You and the publisher haven't committed to a fixed number of impression deliveries. The deal specifies the minimum price for the inventory, although the CPM may fluctuate and increase depending on market conditions.</li><li>[!UICONTROL Non guaranteed (fixed)]: You and the publisher haven't committed to a fixed number of impression deliveries. Pricing is at a negotiated fixed rate.</li><li>[!UICONTROL Guaranteed (fixed)]: You and the publisher have agreed on a pre-defined number of impressions, targeting, flight dates, and fixed price.<br><br><b>Note:</b> Guaranteed deals require flight dates and a specified number of impressions in the [!UICONTROL Tracking] section. You'll also need to create a default programmatic guaranteed (PG) placement for the deal, and you can optionally use the deal for other placements instead.</li></ul>   | Yes  | No |
| | [!UICONTROL CPM] | The negotiated cost per thousand impressions (CPM). | Yes | Yes |
| | [Currency] | The currency for the deal.<br><br>All SSPs accept deals in USD. When the SSP accepts the currency for your DSP account, that currency is also available. | Yes | No |
| | [!UICONTROL Billing method] | All deal IDs are [!DNL Adobe--financed and -invoiced. Advertising Cloud will pay all available media vendors based on usage, manage discrepancies with the vendors, and send one consolidated invoice to the account. This option incurs additional fees as outlined in the account's rate card. | Yes | No |
| [!UICONTROL Advertisers] | [!UICONTROL Account email] | The email address for the user account that can access the deal. | No  | Yes |
| | [!UICONTROL Advertisers that can access this deal] | The specific advertisers in the account who can access this deal.<br><br><b>Note:</b> You can share the deal with advertisers in additional accounts from the [!UICONTROL Deals] view. In the deal row, click **[!UICONTROL #]**, click **[!UICONTROL share]**, and then share the deal with an email address. | Yes | Yes |
| [!UICONTROL Tracking] | [!UICONTROL Flight Dates] | The start and end dates for traffic using this deal. These date are for tracking purposes only and don't impact ad delivery.<br><br><b>Tip:</b> In the [!UICONTROL Inventory] > [!UICONTROL Deals] view, the [!UICONTROL Pacing & Budget] column will show how the deal is pacing to the specified flight date and impression goal. If delivery is under- or over-pacing, contact your publisher to adjust how much volume it is sending through the deal. | Guaranteed deals: Yes<br>Non-guaranteed deals: No | Yes |
| | [!UICONTROL Impressions] | (Optional for non-guaranteed deals) The estimated number of impressions you expect to run using this deal. This value is tracking purposes only; the publisher controls ad delivery. | Guaranteed deals: Yes<br>Non-guaranteed deals: No | Yes |
                         
>[!MORELIKETHIS]
>
>* [Manually Create Deal ID Details](deal-id-create.md)
>* [SSP Partners](ssp-partners.md)
<!-- >* [About Private Inventory](private-inventory-about.md) -->
