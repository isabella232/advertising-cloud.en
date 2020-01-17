---
title: Adobe Advertising Cloud support for the California Consumer Privacy Act &#58; Consumer Opt-out Support
description: Support for capturing consumer opt-out of sale requests
seo-title: Adobe Advertising Cloud support for California Consumer Privacy Act &#58; Consumer Opt-out Support
seo-description: Adobe Advertising Cloud support for capturing consumer opt-out of sale requests
---

# Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Opt-out Support

*For Adobe Advertising Cloud Demand Side Platform*

>[!Important]
>
>The contents of this document are not legal advice and are not meant to substitute for legal advice. Consult with your legal counsel for advice concerning the California Consumer Privacy Act.

The California Consumer Privacy Act (CCPA) is California’s new privacy law, which is effective January 1, 2020. CCPA provides California residents new rights regarding their personal information and imposes data protection responsibilities on certain entities who conduct business in California. CCPA provides consumers with the right to access and delete their data as well as the right to opt out of certain activities that qualify as “selling” personal information to a third party.

As a business, you will determine the personal data that Adobe Experience Cloud processes and stores on your behalf.

As your service provider, Adobe Advertising Cloud provides support for your business to fulfill its obligations under CCPA that are applicable to the use of Advertising Cloud products and services, including managing consumer requests to access and delete personal information and managing consumer requests to opt out of the sale of personal information.

This document describes how Adobe Advertising Cloud Demand Side Platform (DSP), as a service provider, supports the consumer right to opt out of the "sale" of "personal information," as each term is defined by the CCPA.

For information about how Advertising Cloud Search, Advertising Cloud Creative, Advertising Cloud DSP (Demand Side Platform), and Media Optimizer DCO support consumers' personal information access and deletion rights, see [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Data Access and Delete Support](ad-cloud-ccpa-access-delete.md).

For more information about the Adobe Privacy services for CCPA, see the [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Capture Consumer “Opt out of sale” Requests

1. Log into the advertiser's account in Advertising Cloud DSP at [https://www.tubemogul.com](https://www.tubemogul.com).
1. Create a segment to capture the opt-out requests:
   1. In the main menu, select **DSP > Tools > Segments**.
   1. Click **New Custom Segment**.
   1. Enter the segment name, and then click **Save and Close**.

       Recommended segment name: “Your Advertiser Name – CCPA Opt Out of Sale”

1. Locate the new segment in the Segment Manager list, click ![Options menu](assets/edit-menu.png) in the Options column, and then select **get pixel**. <!-- I should be able add hover text in the image link, such as (x.png "hover text"), but either it's not currently supported or it's broken -->
1. Copy the image pixel (beginning with `<img src="https://rtd-tm.everesttech.net"`) to collect user segments that visited a site, and implement the pixel using the mechanism that your company uses to track CCPA opt-out of sale requests (such as using a Consent Management Platform).  

    Once the pixel is implemented, Advertising Cloud will begin to collect a pool of IDs on the advertiser’s behalf.

    Although implementation choice and logic is up to the advertiser, here’s an example of how an advertiser would fire the pixel:

    1. A consumer lands on the advertiser's homepage.
    1. The consumer finds and clicks on the advertiser’s “CCPA opt out of sale” button.
    1. The consumer is presented with a list of service providers with which the advertiser works.
    1. The consumer checks the box to opt out of selling data to Adobe Advertising Cloud.

        This action triggers the pixel to fire and to collect the consumer’s cookie ID within the “CCPA – Opt out of sale”  segment.

1. (Optional) To access the list of cookie IDs that have been added to the “CCPA opted out of sale” segment in your account, contact your Advertising Cloud account manager to request a file export. Include the advertiser name, the email address for the Advertising Cloud account, and the segment name.

    The file may be used as a reference when considering the use of Advertising Cloud campaign data in downstream activities that involve service providers outside of Adobe, for example for segmentation or user profile creation.
