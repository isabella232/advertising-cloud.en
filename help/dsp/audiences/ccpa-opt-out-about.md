# About CCPA Opt-out-of-Sale Segments and Reports

You can track users IDs from consumer opt-out-of-sale requests on your website, per the California Consumer Privacy Act (CCPA), by [creating and implementing a CCPA opt-out-of-sale segment](ccpa-opt-out-segment-create.md). Users remain in CCPA opt-out-of-sale segments indefinitely.

Once the segment pixel tag is implemented, Advertising Cloud will begin to collect a pool of IDs on the advertiser’s behalf.

## Consumer Opt-Out-of-Sale Reports

Advertising Cloud generates monthly reports of IDs that customers have submitted for opt-out-of-sale requests for the account. The data consolidates requests captured using CCPA opt-out-of-sale segments that were created in Advertising Cloud DSP and any submissions made via the Privacy Service API.  Reports are generated on the first of each month for the previous month. For example, the monthly user list for June is available on July 1.

Each report is available as a tab-separated text file compressed into GZIP format. User IDs captured in CCPA opt-out-of-sale segments are identified by segment and by advertiser.

You can [retrieve links to the monthly reports](ccpa-opt-out-segment-report-retrieve.md) that were created in the previous three months, either from within Advertising Cloud DSP or by using the Advertising Cloud Trafficking API. Each link is valid for seven days but refreshes each time a customer attempts to retrieve one.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Opt-out Support](https://docs.adobe.com/content/help/en/advertising-cloud/privacy/ad-cloud-ccpa-opt-out-of-sale.html)
>* [Create and Implement a CCPA Opt-Out-of-Sale Segment](ccpa-opt-out-segment-create.md)
>* [Retrieve Consumer Opt-Out-of-Sale Reports](ccpa-opt-out-segment-report-retrieve.md)
>* [About Audience Management](audience-about.md)
