---
title: Advertising Cloud IDs Used by [!DNL Analytics]
description: Advertising Cloud IDs Used by [!DNL Analytics]
feature: Integration with Adobe Analytics
exl-id: ed1aab7b-9bd0-4d42-9bfb-9c6fa6db76bc
---
# Advertising Cloud IDs Used by [!DNL Analytics]

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

*Applicable to Advertising Cloud DSP and Advertising Cloud Search*

Advertising Cloud uses two IDs for onsite performance tracking:  the *EF ID* and the *AMO ID*.

When an ad impression occurs, Advertising Cloud creates the AMO ID and EF ID values and stores them. When a visitor who has seen an ad enters the site without clicking an ad, [!DNL Analytics] calls these values from Advertising Cloud through the [!DNL Analytics for Advertising Cloud] JavaScript code. For view-through traffic, [!DNL Analytics] generates a supplemental ID (`SDID`), which is used to stitch the EF ID and AMO ID into [!DNL Analytics]. For click-through traffic, these IDs are included in the landing page URL using the `s_kwcid` and `ef_id` query string parameters.

Advertising Cloud distinguishes between a click-through or view-through entry to the website using the following criteria:

* A view-through entry is captured when a user visits the site after viewing an ad but not clicking it. [!DNL Analytics] records a view-through if two conditions are met:
    * The visitor has no click-throughs for a [!DNL DSP] or [!DNL Search] ad during the [click lookback window](#lookback-a4adc).
    * The visitor has seen at least one [!DNL DSP] ad during the [impression lookback window](#lookback-a4adc). The last impression is passed as the view-through.
* A click-through entry is captured when a site visitor clicks an ad before entering the site. [!DNL Analytics] captures a click-through when either of the following conditions occurs:
    * The URL includes an EF ID and AMO ID as added to the landing page URL by Advertising Cloud.
    * The URL contains no tracking codes, but the Advertising Cloud JavaScript code detects a click within the last two minutes.

![Advertising Cloud view-based [!DNL Analytics] integration](/help/integrations/assets/a4adc-view-through-process.png)

*Figure 1: Advertising Cloud view-based [!DNL Analytics] integration*

![Advertising Cloud click URL-based [!DNL Analytics] integration](/help/integrations/assets/a4adc-click-through-process.png)

*Figure 2: Advertising Cloud click URL-based [!DNL Analytics] integration*

## Advertising Cloud EF IDs

The EF ID is a unique token that Advertising Cloud uses to associate activity with an online click or ad exposure. The EF ID is stored in an [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) or rVar (reserved eVar) dimension (Advertising Cloud EF ID) and tracks each ad click or exposure at the individual browser or device level. EF IDs act primarily as keys for sending [!DNL Analytics] data to Advertising Cloud for reporting and bid optimization within Advertising Cloud.

### EF ID Format

```<Advertising Cloud visitor ID>:<timestamp>:<channel type>```

<!-- <*Advertising Cloud visitor ID*>:<*timestamp*>:<*channel type*> -->

where:

* <*Advertising Cloud visitor ID*> is a unique ID per visitor (such as UhKVaAAABCkJ0mDt). Also called the *surfer ID*.

* <*timestamp*> is the time in the format YYYYMMDDHHMMSS (such as 20190821192533 for Year 2019, Month 08, Day 21, Time 19:25:33).

* <*channel type*> is the channel type responsible for the click or exposure:

    * `d` for a click on a DSP display ad (display click-through)
    * `i` for an impression of a DSP display ad (display view-through)
    * `s` for a click on a Search ad (search click-through).

Example `EF `ID: WcmibgAAAHJK1RyY:1551968087687:d

>[!NOTE]
>
>EF IDs are case-sensitive. If an [!DNL Analytics] implementation forces URL tracking to lowercase, then Advertising Cloud will not recognize the EF ID. This will impact Advertising Cloud bidding and reporting but has no impact on Advertising Cloud reporting within [!DNL Analytics].

### The EF ID Dimension in [!DNL Analytics]

In [!DNL Analytics] reports, you can find EF ID data by searching for the [!UICONTROL EF ID] dimension and using the [!UICONTROL EF ID Instance] metric.

EF IDs are subject to the 500k unique identifier limit in Analysis Workspace. Once the 500k value is reached, all new tracking codes are reported under the one-line-item title “[!UICONTROL Low Traffic].” Because of the possibility of missing reporting fidelity, the EF IDs are not classified, and you should not use them for segments or reporting in [!DNL Analytics].

## Advertising Cloud AMO IDs

The AMO ID tracks each unique ad combination at a less granular level and is used for [!DNL Analytics] data classification and ingestion of advertising metrics (such as impressions, clicks, and cost) from Advertising Cloud. The AMO ID is stored in an [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) or rVar dimension (AMO ID) and is used exclusively for reporting in [!DNL Analytics].

The AMO ID is also called the `s_kwcid`, which is sometimes pronounced as "[!DNL the squid]."

### AMO ID Format for [!DNL DSP]

```<Channel ID>!<Ad ID>!<Placement ID>```

where:

* <*Channel ID*> may be:

    * `AC` = Advertising Cloud DSP
    * `AL` for Advertising Cloud Search

* <*Ad ID*> is used an Advertising Cloud-generated unique identifier for an ad. It serves as a key for translating Advertising Cloud entity metadata into readable [!DNL Analytics] dimensions.

* <*Placement ID*> is an Advertising Cloud-generated unique identifier for an placement. It serves as a key for translating Advertising Cloud entity metadata into readable [!DNL Analytics] dimensions.

<!-- <*Channel ID*>!<*Ad ID*>!<*Placement ID*>

where:

* <*Channel ID*> may be:

    * `AC` = Advertising Cloud DSP
    * `AL` for Advertising Cloud Search

* <*Ad ID*> is used an Advertising Cloud-generated unique identifier for an ad. It serves as a key for translating Advertising Cloud entity metadata into readable [!DNL Analytics] dimensions.

* <*Placement ID*> is an Advertising Cloud-generated unique identifier for an placement. It serves as a key for translating Advertising Cloud entity metadata into readable [!DNL Analytics] dimensions.
 -->

Example AMO ID: AC!iIMvXqlOa6Nia2lDvtgw!GrVv6o2oV2qQLjQiXLC7

### AMO ID Format for [!DNL Search]

AMO IDs for [!DNL Search] follow a distinct format for each search engine. The format for all search engines begins with the following:

```AL!{ef_userid}!{ef_sid}```

where:

* `AL` is the channel ID for the search channel.
* `{ef_userid}` is the unique numeric user ID that Advertising Cloud assigns to the advertiser.
* `{ef_sid}` is the numeric ID that Advertising Cloud uses for the specified search engine, such as `3` for [!DNL Google Ads] or `10` for [!DNL Microsoft Advertising].

The following are the full AMO ID formats for a couple of search engines. For AMO ID formats for other search engines, contact your [!DNL Adobe] account team.

AMO ID Format for [!DNL Google Ads]:

```AL!{ef_userid}!{ef_sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}```

where:

* `{creative}` is the [!DNL Google Ads] unique numeric ID for the creative.
* `{matchtype}` is the matchtype of the keyword that triggered the ad: `e` for exact, `p` for phrase, or `b` for broad.
* `{placement}` is the domain name of the website on which the ad was clicked. A value is available for ads in placement-targeted campaigns and for ads in keyword-targeted campaigns that are displayed on content sites.
* `{network}` indicates the network from which the click occurred:  `g` for [!DNL Google] search (for keyword-targeted ads only), `s` for a search partner (for keyword-targeted ads only), or `d` for the Display Network (for either keyword-targeted or placement-targeted ads).
* `{keyword}` is either the specific keyword that triggered your ad (on search sites) or the best-matching keyword (on content sites).

AMO ID Format for [!DNL Microsoft Advertising]:

```AL!{ef_userid}!{ef_sid}!{AdId}!{OrderItemId}```

where:

* `{AdId}` is the [!DNL Microsoft Advertising] unique numeric ID for the creative.
* `{OrderItemId}` is the [!DNL Microsoft Advertising] numeric ID for the keyword.

### AMO ID Dimension in [!DNL Analytics]

In Analytics reports, you can find AMO ID data by searching for the [!UICONTROL AMO ID] dimension and using the [!UICONTROL AMO ID Instance] metric. The [!UICONTROL AMO ID] dimension houses all AMO ID values captured, whereas the [!UICONTROL AMO ID Instance] metric indicates how often an AMO ID value was captured by the site. For example, if the same search ad was clicked four times but Analytics tracked seven site entries, then [!UICONTROL AMO ID Instance] would be seven (7) and [!UICONTROL Clicks] would be four (4).

For any reporting or auditing within [!DNL Analytics], the best practice is to use the AMO ID along with its corresponding instance. For more information, see "[Data Validation for [!DNL Analytics for Advertising Cloud]](data-variances.md#data-validation)" in "Expected Data Variances Between [!DNL Analytics] and Advertising Cloud."

## About Analytics Classifications

In [!DNL Analytics], a [classification](https://experienceleague.adobe.com/docs/analytics/components/classifications/c-classifications.html) is a piece of metadata for a given tracking code, such as Account, Campaign, or Ad. Advertising Cloud categorizes raw Advertising Cloud data using classifications so that you can display the data in different ways (such as by Ad Type or Campaign) when you generate reports. Classifications form the basis of Advertising Cloud reporting in [!DNL Analytics] and can be used with the AMO metrics, such as [!UICONTROL AMO Cost], [!UICONTROL AMO Impressions], and [!UICONTROL AMO Clicks], as well as with custom and standard  onsite events like [!UICONTROL Visits], [!UICONTROL Leads], [!UICONTROL Orders], and [!UICONTROL Revenue].

>[!MORELIKETHIS]
>
>* [Overview of [!DNL Analytics for Advertising Cloud]](overview.md)
>* [Expected Data Variances Between [!DNL Analytics] and Advertising Cloud](data-variances.md)
