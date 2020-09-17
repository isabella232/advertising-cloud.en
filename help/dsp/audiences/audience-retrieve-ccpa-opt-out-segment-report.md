# Retrieve Consumer Opt-Out-of-Sale Reports {#audience-retrieve-ccpa-opt-out-segment-report}

Advertising Cloud generates monthly reports of IDs that customers have submitted for opt-out-of-sale requests for the account. Each report is available as a tab-separated text file compressed into GZIP format. The data consolidates requests captured using CCPA opt-out-of-sale segments and any submissions made via the Privacy Service API. User IDs captured in CCPA opt-out-of-sale segments created in Advertising Cloud are identified by segment and by advertiser. Reports are generated on the first of each month for the previous month. For example, the monthly user list for June is available on July 1.

You can retrieve links to the monthly reports that were created in the previous three months, either from within Advertising Cloud or by using the Advertising Cloud Trafficking API. Each link is valid for seven days but refreshes each time a customer attempts to retrieve one.

>[!NOTE]
>
>To retrieve consumer opt-out-of-sale reports using the Advertising Cloud Trafficking API, see the documentation for the Trafficking API. If your organization doesn't use the Trafficking API but is interested in more information, contact your Adobe account manager.

1. In the main menu, select **Audiences > Segments**.
1. Above the segment list, click **Access CCPA Reports**.
1. Click the link for any available monthly report to download a GZIP file, which you can extract to a tab-separated text file.

>[!MORELIKETHIS]
>
>* [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Opt-out Support](https://docs.adobe.com/content/help/en/advertising-cloud/all/privacy/ad-cloud-ccpa-opt-out-of-sale.html)
>* [Create and Implement a Custom Segment](audience-create-custom-segment.md)
>* [About Audience Management](audience-about.md)
