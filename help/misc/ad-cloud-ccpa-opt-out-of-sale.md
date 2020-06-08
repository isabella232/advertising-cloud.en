---
title: Adobe Advertising Cloud support for the California Consumer Privacy Act &#58; Consumer Opt-out Support
description: Support for capturing consumer opt-out of sale requests
---

# Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Opt-out Support

*For Adobe Advertising Cloud Demand Side Platform*

>[!IMPORTANT]
>
>The contents of this document are not legal advice and are not meant to substitute for legal advice. Consult with your legal counsel for advice concerning the California Consumer Privacy Act.

The California Consumer Privacy Act (CCPA) is California’s new privacy law, which is effective January 1, 2020. CCPA provides California residents new rights regarding their personal information and imposes data protection responsibilities on certain entities who conduct business in California. CCPA provides consumers with the right to access and delete their data as well as the right to opt out of certain activities that qualify as “selling” personal information to a third party.

As a business, you will determine the personal data that Adobe Experience Cloud processes and stores on your behalf.

As your service provider, Adobe Advertising Cloud provides support for your business to fulfill its obligations under CCPA that are applicable to the use of Advertising Cloud products and services, including managing consumer requests to access and delete personal information and managing consumer requests to opt out of the sale of personal information.

This document describes how Adobe Advertising Cloud Demand Side Platform (DSP), as a service provider, supports the consumer right to opt out of the "sale" of "personal information," as each term is defined by the CCPA. It includes information on how to communicate opt-out-of-sale requests to Advertising Cloud and how to retrieve reports of your organization's opt-out-of-sale requests.

For information about how Advertising Cloud Search, Advertising Cloud Creative, Advertising Cloud DSP (Demand Side Platform), and Media Optimizer DCO support consumers' personal information access and deletion rights, see [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Data Access and Delete Support](ad-cloud-ccpa-access-delete.md).

For more information about the Adobe Privacy services for CCPA, see the [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Communicating Consumer Opt-out-of-sale Requests to Advertising Cloud

You can communicate consumer opt-out-of-sale requests by using either:

* a CCPA opt-out-of-sale segment created in Advertising Cloud
* the Adobe Experience Platform Privacy Service API

### Method 1: Capture CCPA Opt-Out-of-Sale Requests Using a CCPA Opt-out-of-sale Segment

1. Log into the advertiser's account in Advertising Cloud DSP at [https://www.tubemogul.com](https://www.tubemogul.com).
1. Create a segment to capture the opt-out requests:
   1. In the main menu, select **Audiences > Segments**.
   1. Click **Create**.
   1. Enter the segment name, and then click **Save and Close**.

       Recommended segment name: “Your Advertiser Name – CCPA Opt Out of Sale”

1. In the Segments list, hold the cursor over the new segment and click **Get pixel**.
1. Copy the image pixel (beginning with `<img src="https://rtd-tm.everesttech.net"`) to collect user segments that visited a site, and implement the pixel using the mechanism that your company uses to track CCPA opt-out of sale requests (such as using a Consent Management Platform).  

    Once the pixel is implemented, Advertising Cloud will begin to collect a pool of IDs on the advertiser’s behalf.

    Although implementation choice and logic is up to the advertiser, here’s an example of how an advertiser would fire the pixel:

    1. A consumer lands on the advertiser's homepage.
    1. The consumer finds and clicks on the advertiser’s “CCPA opt out of sale” button.
    1. The consumer is presented with a list of service providers with which the advertiser works.
    1. The consumer checks the box to opt out of selling data to Adobe Advertising Cloud.

        This action triggers the pixel to fire and to collect the consumer’s cookie ID within the “CCPA – Opt out of sale”  segment.

### Method 2: Capture CCPA Opt-out-of-Sale Requests Using the Adobe Experience Platform Privacy Service API

*Advertisers assigned an Experience Cloud Organization ID (IMS Org ID) only*

1. Deploy a JavaScript library to retrieve and remove your customer's cookies. The same library, AdobePrivacy.js, is used for all Adobe Experience Cloud solutions.

   >[!IMPORTANT]
   >
   >Requests to some Adobe Experience Cloud solutions don't require the JavaScript library, but requests to Advertising Cloud require it.

   You should deploy the library on the web page from which your customers can submit opt-out-of-sale requests, such as your company's privacy portal. The library helps you retrieve Adobe cookies (namespace ID: gsurferID) so that you can submit these identities as part of opt-out-of-sale requests via the Adobe Experience Platform Privacy Service API.

1. Identify your IMS Org ID and make sure it is linked to your Advertising Cloud accounts.

   An IMS Org ID is a 24-character alphanumeric string appended with @AdobeOrg. Most Adobe Experience Cloud customers have been assigned an IMS Org ID. If your marketing team or internal Adobe system administrator doesn't know your organization's IMS Org ID, or isn't sure if it's been provisioned, contact Adobe Customer Care at gdprsupport@adobe.com. You'll need the IMS Org ID to submit requests to the Privacy API.

   >[!IMPORTANT]
   >
   >Contact your company’s Advertising Cloud representative to confirm that all of your organization's Advertising Cloud accounts &mdash; including DSP accounts or advertisers, Search accounts, and Creative or DCO accounts &mdash; are linked to your IMS Org ID.

1. Use the Adobe Experience Platform Privacy Service API to submit opt-out-of-sale requests to Advertising Cloud on behalf of consumers, and to check the status of existing requests.

   For advertisers who have a mobile app to interact with customers and launch campaigns with the DSP, you'll need to download the Privacy-ready Mobile SDKs for Experience Cloud. The Mobile SDKs allow businesses to set opt-out status flags, retrieve the consumer's device ID (namespace ID: deviceID), and submit requests to the Privacy Service API. Your mobile app will require an SDK Version 4.15.0 or greater.

   >[!NOTE]
   >
   >If your business has multiple Adobe Experience Cloud Identity Management Service Organization IDs (IMS Org IDs), then you must send separate API requests for each. You can, however make one API request to multiple Advertising Cloud sub-solutions (Search, Creative, DSP, and DCO), with one account per sub-solution.

All of these steps are necessary to receive support from Advertising Cloud. For more information about these and other related tasks you need to perform using the Adobe Experience Platform Privacy Service, and where to find the items you'll need, see [https://docs.adobe.com/content/help/en/experience-platform/privacy/home.html](https://docs.adobe.com/content/help/en/experience-platform/privacy/home.html).

## Retrieving Reports of Consumers Who Submitted Opt-out-of-sale Requests

Advertising Cloud generates monthly reports of users who submitted opt-out-of-sale requests for the account, as comma-separated values (CSV) files in ZIP format. The data consolidates requests captured using CCPA opt-out-of-sale segments and any submissions made via the Privacy Service API, and it includes cookie IDs by segment and advertiser. Reports are generated on the first of each month for the previous month. For example, the monthly user list for June is available on 1 July.

You can retrieve links to the monthly reports that were created in the previous three months, either from within Advertising Cloud or by using the Advertising Cloud Trafficking API. Each link is valid for seven days. After the links expire, you can retrieve new links.

### Method 1: Retrieve Consumer Opt-out-of-Sale Reports Within Advertising Cloud

1. Log into the advertiser's account in Advertising Cloud DSP at [https://www.tubemogul.com](https://www.tubemogul.com).

1. In the main menu, select **Audiences > Segments**.

1. Above the segment list, click **Access CCPA Reports**.

1. Click the link for any monthly report to download a ZIP file that you can extract to CSV format. <!-- verify -->

### Method 2: Retrieve Consumer Opt-out-of-Sale Reports Using the Advertising Cloud Trafficking API

This feature is available to organizations that use the Trafficking API. See the documentation for the Trafficking API for more information.

If your organization doesn't use the Trafficking API but is interested in more information, contact your Adobe account manager.

## Appendix: Required Values and Examples for Privacy Service API Users

TBD
