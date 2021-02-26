# Expected Data Variances Between Analytics and Advertising Cloud

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

Advertisers with the Analytics for Advertising Cloud <!-- (A4AdC) --> integration track paid advertising through Advertising Cloud and Adobe Analytics. When you track media, campaigns, and channels via multiple systems, the same data sets from different systems rarely match completely. This document explains how you should expect data for media that's trafficked through Advertising Cloud to compare to data in the different systems in which the media is tracked within Analytics.

>[!NOTE]
>
>This document is focused on Advertising Cloud and Analytics, but many of the key points are also transferable to other tracking solutions.

## Attribution Differences in Similar Reports

### Potentially Different Lookback Windows and Attribution Models

The Analytics for Advertising Cloud integration uses two variables (eVars or rVars \[reserved eVars]\) to capture the [EF ID and AMO ID](ids.md). These variables are configured with a single lookback window (the time within which click-throughs and view-throughs are attributed) and an attribution model. Unless otherwise specified, the variables are configured to match the default, advertiser-level click lookback window and attribution model in Advertising Cloud.

However, lookback windows and attribution models are configurable in both Analytics (via the eVars) and in Advertising Cloud. Further, in Advertising Cloud, the attribution model is configurable not only at the advertiser level (for bid optimization) but also within individual data views and reports (for reporting purposes only). For example, an organization may prefer to use the even distribution attribution model for optimization but use last touch attribution for reports in Advertising Cloud DSP or Search. Changing attribution models changes the number of attributed conversions.

If a reporting lookback window or attribution model is modified in one product and not in the other, then the same reports from each system will show distinct data:

* **Example of discrepancies caused by different lookback windows:**

     Suppose Advertising Cloud has a 60-day click lookback window and Analytics has a 30-day lookback window. And suppose that a user comes to the site through an Advertising Cloud-tracked ad, leaves, and then returns on day 45 and converts. Advertising Cloud will attribute the conversion to the initial visit because the conversion occurred within the 60-day lookback window. Analytics, however, can't attribute the conversion to the initial visit because the conversion occurred after the 30-day lookback window had expired. In this example, Advertising Cloud would report a higher number of conversions than Analytics would.
     
     ![Example of a conversion attributed in Advertising Cloud but not Analytics](/help/dsp/assets/a4adc-lookback-example.png)

* **Example of discrepancies caused by different attribution models:**

     Suppose a user interacts with three different Advertising Cloud ads before converting, with revenue as the conversion type. If an Advertising Cloud report uses an even distribution model for attribution, then it will attribute the revenue evenly across all ads. If Analytics uses the last touch attribution model, however, then it will attribute the revenue to the last ad. In the following example, Advertising Cloud attributes an even 10 USD of the 30 USD of revenue captured to each of the three ads, whereas Analytics attributes all 30 USD of revenue to the last ad seen by the user. When you compare reports from Advertising Cloud and Analytics, you can expect to see the impact of the difference in attribution.
     
     ![Different revenue attributed to Advertising Cloud and Analytics based on different attribution models](/help/dsp/assets/a4adc-attribution-example.png)

>[!IMPORTANT]
>
>The best practice is to use the same lookback windows and attribution model in both Advertising Cloud and Analytics. Work with your Adobe account manager as necessary to identify the current settings and to keep the configurations in sync.

These same concepts apply to any other like channels that use different lookback windows or attribution models.

#### Different Lookback Windows for View-Through Tracking {#impression-lookback}

In Advertising Cloud, attribution is based on clicks and impressions, and you can configure different lookback windows for clicks and for impressions. In Analytics, however, attribution is based on click-throughs and view-throughs, and you don't have the option to set different attribution windows for click-throughs and view-throughs; tracking for each starts at the initial site visit. An impression can occur the same day or multiple days before a view-through occurs, and this can impact where the attribution window starts in each system.

Typically, the majority of view-through conversions occur quickly enough that both systems attribute credit. However, some conversions may occur outside the Advertising Cloud impression lookback window but within the Analytics lookback window; such conversions are attributed to the view-through in Analytics but not to the impression in Advertising Cloud.

In the following example, suppose a visitor was served an ad on Day 1, performed a view-through visit (that is, visited the ad's landing page without previously clicking the ad) on Day 2, and converted on Day 45. In this case, Advertising Cloud would track the user from Days 1–14 (using a 14-day lookback), Analytics would track the user from Days 2–61 (using a 60-day lookback), and the conversion on Day 45 would be attributed to the ad within Analytics but not within Advertising Cloud.

![Example of a view-through conversion attributed in Analytics but not Advertising Cloud](/help/dsp/assets/a4adc-viewthrough-example.png)

A further cause of discrepancies is that, in Advertising Cloud, you can assign view-through conversions a custom *view-through weight* that is relative to the weight attributed to a click-based conversion. The default view-through weight is 40%, which means that a view-through conversion is counted as 40% of the value of a click-based conversion. Analytics provides no such weighting of view-through conversions. So, for example, a 100 USD revenue order captured in Analytics will be discounted to 40 USD in Advertising Cloud if you're using the default view-through weight &mdash; a difference of 60 USD.

Consider these differences when comparing view-through conversions between Advertising Cloud and Analytics reports.

#### Available Attribution Models

| Advertising Cloud Attribution | Analytics Attribution | eVar/rVar Allocation |
|--- |--- |--- |
| Last Event | Last Touch | Most Recent |
| First Event | First Touch | Original Value |
| Weight First Event More | n/a | n/a |
| Even Distribution | Linear | Linear<br><br>Don't Use* |
| Weight Last Event More | n/a | n/a |
| U-Shaped | U-Shaped | n/a |
| n/a | J-Shaped | n/a |
| n/a | Inverse-J | n/a |
| n/a | Custom | n/a |
| n/a | Participation | n/a |
| n/a | Algorithmic | n/a |

>[!NOTE]
>
>For linear allocation, Analytics attributes success events equally across all eVar values within a single visit, so use linear allocation with an eVar expiration of "Visit." For advertising, however, the use of linear attribution leads to allocation that is not truly linear and to less-than-ideal reporting. For example, if a visitor interacts with three ads before converting in three separate visits, only the ad seen in the last visit is attributed to the conversion, not all three ads.
>
>In addition, switching conversion allocation to or from "Linear" prevents historical data from displaying, which can can lead to misstated data in reports. For example, linear allocation might divide revenue across a number of different eVar values. If you change allocation to "Most Recent," then 100% of that revenue becomes associated with the most recent single value. This association can lead you to incorrect conclusions.
>
>To prevent confusion, Analytics makes historical data unavailable in the reporting interface. You can view the historical data if you change the eVar back to the initial allocation setting, although you should not change eVar allocation settings simply to access historical data. Adobe recommends using a new eVar when you want to apply a new allocation setting for data that's already being recorded, rather than changing allocation settings for an eVar that already has a significant amount of historical data.

See a list of Analytics attribution models and their definitions at https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/attribution/models.html.

If you're logged into Advertising Cloud, you can find a list of attribution models at
https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm

#### Event Date Attribution in Advertising Cloud

In Advertising Cloud, you can report conversion data either by the associated click date/event date (the date of the click or impression event) or by the transaction date (conversion date). The concept of click/event date reporting doesn't exist in Analytics; all conversions tracked in Analytics are reported by transaction date. As a result, the same conversion may be reported with different dates in Advertising Cloud and Analytics. For example, consider a user who clicks an ad on January 1 and converts on January 5. If you're viewing the conversion data by event date in Advertising Cloud, then the conversion will be reported on January 1, when the click occurred. In Analytics, the same conversion would be reported on January 5.

![Example of a conversion attributed to different dates](/help/dsp/assets/a4adc-conversions-based-on.png)

## Attribution in Analytics Marketing Channels

Analytics [Marketing Channels](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/marketing-channels-admin.html) reporting allows you to configure rules to identify different marketing channels based on distinct aspects of hit information. You can track Advertising Cloud-tracked channels (Display Click Through, Display View Through, and Paid Search) as Marketing Channels by using the "ef_id" query string parameter to identify the channel. <!-- Move most of the above text to "Marketing Channels" chapter once it's created, and add link here. --> However, even though the Marketing Channels reports can track Advertising Cloud channels, the data may not match the Advertising Cloud reports for several reasons. See the following sections for more information.

>[!NOTE]
>
> The following core concepts also apply to any multi-channel tracking that involves campaigns not tracked in Advertising Cloud, such as the "[campaign](https://experienceleague.adobe.com/docs/analytics/implementation/vars/page-vars/campaign.html)" variable (also known as the "Tracking code" Dimension or "eVar 0") and custom eVar tracking.

### Potentially Different Attribution Models in Marketing Channels

Most Marketing Channels reports are configured with Last Touch attribution, for which the last marketing channel detected is assigned 100% of the conversion value. Using different attribution models for the Marketing Channel reports and Advertising Cloud reports will lead to discrepancies in attributed conversions.

### A Potentially Different Lookback Window in Marketing Channels

The lookback window for Marketing Channels can be customized. In Advertising Cloud, the click lookback window is configurable, although a fixed 60-day window is common. If the two products use different lookback windows, you can expect data discrepancies.

### Different Channel Attribution in Marketing Channels

Advertising Cloud reports capture only paid media trafficked through Advertising Cloud (paid search for Advertising Cloud Search ads, and display for Advertising Cloud DSP ads), whereas Marketing Channels reports can track all digital channels. This can lead to a discrepancy in the channel for which a conversion is attributed.

For example, paid search and natural search channels often have a symbiotic relationship, in which each channel assists the other. The Marketing Channels report will attribute some conversions to natural search that Advertising Cloud won't because it doesn't track natural search.

Consider also a customer who views a display ad, clicks a paid search ad, clicks inside an email message, and then places a 30 USD order. Even if Advertising Cloud and Marketing Channels both use the last touch attribution model, the conversion would still be attributed differently to each. Advertising Cloud doesn't have access to the email channel, so it would credit paid search for the conversion. Marketing Channels, however, has access to all three channels, so it would credit email for the conversion.

![Example of different conversion attribution in Advertising Cloud versus Analytics Marketing Channels](/help/dsp/assets/a4adc-channel-example.png)

## Data Differences in Adobe Analytics Paid Search Detection

[Paid Search Detection](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/paid-search-detection/paid-search-detection.html) is a legacy feature in Analytics that allows companies to [define rules to track paid and organic search traffic](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/paid-search-detection/t-paid-search-detection.html) for specified search engines. The Paid Search Detection rules use both a query string and the referring domain to identify paid and natural search traffic. The Paid Search Detection reports are part of the larger group of [Finding Methods](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/finding-methods.html) reports, which expire either when a specified event (such as a Cart Checkout) occurs or the visit ends.

The following is the interface for creating a Paid Search Detection rule set:

![Example of a Paid Search Detection rule set in Analytics](/help/dsp/assets/a4adc-paid-search-detection.png)

The resulting Paid Search Detection reports include the Paid Search Engine, Paid Search Keywords, Natural Search Engine, and Natural Search Keywords reports.

Note the following two limitations with data in Paid Search Detection reports:

* The Paid Search Keywords and Natural Search Keywords reports show the search queries as identified by the referring URLs, not the keywords on which users bid. Advertising Cloud and Analytics reports show the actual keywords, so don't expect them to align with the Paid Search Detection keyword reports.

* When the Paid Search Detection feature was originally created, the originating search query (the string of characters the user entered into the search bar in the search engine) was more readily available to advertisers via the referring URL. Today, search engines largely obfuscate the search query, and the Paid Search Detection keyword reports are of limited value because most query data falls under "unspecified."

     With Analytics for Advertising Cloud, advertisers can still track paid keywords in Analytics. The referring domain informs the engine reports which search engine drove the traffic. Since the advertiser-specific account information isn’t tied to the referring domain, all traffic is listed under the search engine. Advertisers with multiple accounts in the same search engine should refer to Advertising Cloud or Analytics reporting for account-specific reporting.

### Why Configure Paid Search Detection?

The Paid Search Detection reports allow you to identify natural search traffic in the Analytics [Marketing Channels](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/marketing-channels-admin.html) reports. Separating paid search traffic versus natural search traffic is a great way to understand the value that natural search brings to the full marketing ecosystem.

## Click-Through Data Validation for Analytics for Advertising Cloud{#data-validation}

For your integration, you should validate your click-through data to make sure that all pages on your site are properly tracking click-throughs.

In Analytics, one of the easiest ways to validate Analytics for Advertising Cloud tracking is to compare clicks to instances using the "Clicks to AMO ID Instances" calculated metric, which is calculated as follows:

```Clicks to AMO ID Instances = (AMO ID Instances / AMO Clicks)```

AMO ID Instances represents the number of times AMO IDs (s_kwcid parameters) are tracked on the site. Each time an ad is clicked, a s_kwcid parameter is added to the landing page URL. The number of AMO ID Instances, therefore, is analogous to the number of clicks and can be validated against actual ad clicks. We typically see an 80% match rate for Search and a 30% match rate for DSP traffic (when filtered to include only click-through AMO ID Instances). The difference in expectations between search and display can be explained by the expected traffic behavior. Search captures intent, and, as such, users usually intend to click on the search results from their query. Users who see a display or online video ad, however, are more likely to click the ad unintentionally and then either bounce from the site or abandon the new window that loads before the page activity is tracked.

In Advertising Cloud reports, you can similarly compare clicks to instances using the "ef_id_instances" metric instead of AMO ID Instances:

```Clicks to EF ID Instances = (ef_id_instances / Clicks)```

While you should expect a high match rate between the AMO ID and the EF ID, don't expect 100% parity because AMO ID and EF ID fundamentally track different data, and this difference can lead to slight differences in the total AMO ID Instances and EF ID Instances. If the total AMO ID Instances in Analytics differ from EF ID Instances in Advertising Cloud by more than 1%, however, contact your Adobe account manager for assistance.

For more information about the AMO ID and EF ID, see [Advertising Cloud IDs Used by Analytics](ids.md).

The following is an example of a workspace to track clicks to instances.

![Example of a workspace to track clicks to instances](/help/dsp/assets/a4adc-clicks-to-instances-example.png)
 
## Comparing Data Sets in Analytics for Advertising Cloud Versus in Advertising Cloud

The [AMO ID](ids.md) (s_kwcid query string parameter) is used for reporting in Analytics, and the [EF ID](ids.md) is used for reporting in Advertising Cloud. Because they're distinct values, it's possible for one value to be corrupted or not added to the landing page.

For example, suppose we have the following landing page:

www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id

where the EF ID is "test_ef_id" and the AMO ID is "test_amo_id."

If a site-side redirect occurs, then the URL could end up like this:

www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id#redirectAnchorTag

where the EF ID is "test_ef_id" and the AMO ID is "test_amo_id#redirectAnchorTag."

In this example, the addition of the anchor tag adds unexpected characters to the AMO ID, resulting in a value that Analytics doesn't recognize. This AMO ID wouldn't be classified, and conversions associated with it would fall under "unspecified" or "none" in Analytics reports.

Fortunately, while issues like this are common, they typically don't result in a high percentage of discrepancy. However, if you notice a large discrepancy between AMO IDs in Analytics and EF IDs in Advertising Cloud, contact your Adobe account manager for assistance.

## Other Metric Considerations

### The Difference Between Clicks and Visits {#clicks-vs-visits}

They seem analogous, but clicks and visits represent different data:

* **Click:** DSP or the search engine records a click when a visitor clicks an ad on a publisher’s website.

* **Visit:** Analytics defines a [visit](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html) as a series of page views by a user, ending according to to one of several criteria, such as 30 minutes of inactivity.

By definition, a click can lead to multiple visits.

Consider the following example: User 1 and User 2 both access a site by clicking an Advertising Cloud ad. User 1 views four pages and then leaves for the day, so the initial click results in one visit. User 2 views two pages, leaves for a 45-minute lunch, returns, views two more pages, and then leaves; in this case, the initial click results in two visits.

![Example of the difference between clicks and visits](/help/dsp/assets/a4adc-visits-example.png)

### The Difference Between Clicks and Click-Throughs
<!-- Rob to let me know if we should remove this and add more info. to the section on AMO Instances etc. -->

Clicks and click-throughs are two different metrics:

* **Click:** DSP or the search engine records a click when a visitor clicks an ad on a publisher’s website.

* **Click-throughs:** Analytics records a click-through when the visitor lands on the destination website, the landing page loads, and the Analytics request at the bottom of the page sends the data to Analytics.

Clicks and click-throughs can differ greatly because of accidental ad clicks. We've observed that most clicks on display ads are accidental clicks, and these accidental visitors hit the Back button before the landing page loads, so Analytics isn't able to record a click-through. This is especially true for ads on which an accidental click is more likely, such as mobile ads, video ads, and ads that fill the screen and must be closed before the user can view the page.

Sites loaded on mobile devices are also less likely to result in click-throughs because of lower bandwidths or available processing power, causing landing pages to take longer to load. It's not uncommon for 50-70% of clicks to not result in click-throughs. In mobile environments, the difference can be as high as 90% because of the combination of a slower browser and the higher likelihood that the user accidentally clicks the ad while scrolling through the page or trying to close the ad.

The click data may also be recorded in environments that can't record click-throughs with the current tracking mechanisms (such as clicks going into, or from, a mobile app) or for which the advertiser deployed only one tracking approach (for example, with the view-through JavaScript approach, browsers that block third-party cookies will track clicks, but not click-throughs). A key reason that Adobe recommends deploying both the click URL tracking and view-through JavaScript tracking approaches is to maximize coverage of trackable click-throughs.

### Using Advertising Cloud Traffic Metrics for Non-Advertising Cloud Dimensions

Advertising Cloud provides Analytics with [advertising-specific traffic metrics  and the related dimensions from DSP and Search](advertising-cloud-metrics-in-analytics.md). The Advertising Cloud-provided metrics are applicable only to the specified Advertising Cloud dimensions, and data isn't available for other dimensions in Analytics.

For example, if you view the AMO Clicks and AMO Cost metrics by Account, which is an Advertising Cloud dimension, then you'll see the total AMO Clicks and AMO Cost by account.

![Example of Advertising Cloud metrics in a report using an Advertising Cloud dimension](/help/dsp/assets/a4adc-traffic-supported-dimension.png)

However, if you view the AMO Clicks and AMO Cost metrics by an on-page dimension (such as Page), for which which Advertising Cloud doesn't provide data, then the AMO Clicks and AMO Cost for each page will be zero (0).

![Example of Advertising Cloud metrics in a report using an unsupported dimension](/help/dsp/assets/a4adc-traffic-unsupported-dimension.png)

### Using AMO ID Instances as a Substitute for Clicks with Non-Advertising Cloud Dimensions

Since you can't use AMO Clicks with on-site dimensions, you may want to find an equivalent to clicks. You may be tempted to use Visits as a substitute, but they aren't the best option because each visitor may have multiple visits. (See "[The Difference Between Clicks and Visits]( {#clicks-vs-visits}.") Instead, we recommend using AMO ID Instances, which is the number of times the AMO ID is captured. While AMO ID Instances won't match AMO Clicks exactly, they are the best option for measuring click traffic on the site. For more information, see "[Data Validation for Analytics for Advertising Cloud](#data-validation)."

![Example of AMO ID Instances instead of AMO Clicks for an unsupported dimension](/help/dsp/assets/a4adc-amo-id-instances.png)

>[!MORELIKETHIS]
>
>* [Overview of Analytics for Advertising Cloud](overview.md)
>* [Advertising Cloud IDs Used by Analytics](/help/dsp/integrations/analytics/ids.md)
>* [Advertising Cloud Metrics in Analysis Workspace](/help/dsp/integrations/analytics/advertising-cloud-metrics-in-analytics.md)
>* [Analytics Data in Advertising Cloud](/help/dsp/integrations/analytics/analytics-data-in-advertising-cloud.md)
