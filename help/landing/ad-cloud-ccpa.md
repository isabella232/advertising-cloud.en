# Adobe Advertising Cloud Support for the California Consumer Privacy Act

*For Adobe Advertising Cloud Search, Adobe Advertising Cloud Creative, Adobe Advertising Cloud DSP, and Legacy Adobe Media Optimizer DCO*

**Important:** The contents of this document are not legal advice and are not meant to substitute for legal advice. Consult your company’s legal department for advice concerning the California Consumer Privacy Act.

The California Consumer Privacy Act (CCPA) is California’s new privacy law, which is effective January 1, 2020. CCPA provides California residents new rights regarding their personal information and imposes data protection responsibilities on certain entities who conduct business in California. CCPA provides consumers with the right to access and delete their data as well as the right to opt out of certain activities that qualify as “selling” personal information to a third party.

As a business, you will determine the personal data that Adobe Experience Cloud processes and stores on your behalf.

This document describes how Advertising Cloud Search, Advertising Cloud Creative, Advertising Cloud DSP (Demand Side Platform), and legacy Media Optimizer DCO support consumers' data access and deletion rights using the Adobe Experience Platform Privacy Service API and Privacy Service UI.

For more information about what CCPA means for you, see the [Adobe Privacy Center](https://www.adobe.com/privacy.html).

## Supported Data Request Types for Advertising Cloud

Adobe Experience Platform provides the ability for businesses to complete the following tasks:

* Access a consumer's cookie-level data or device ID-level data (for ads in mobile apps) within Search, Creative, DSP, or DCO.
* Delete cookie-level data stored within Search, Creative, DSP, or DCO for consumers using a browser; or delete ID-level data stored within DSP for consumers using apps on mobile devices.
* Check the status of one or all existing requests.

>[!NOTE]
>
>If your company has multiple Adobe Experience Cloud Identity Management Service Organization IDs (IMS Org IDs), then you must send separate API requests for each. You can, however make one API request to multiple Advertising Cloud sub-solutions (Search, Creative, DSP, and DCO), with one account per sub-solution.

## Required Setup to Send Requests for Advertising Cloud

To make requests to access and delete data for Advertising Cloud, you'll need to:

1. Deploy a lightweight JavaScript library to retrieve and remove your customer's cookies. The same library, AdobePrivacy.js, is used for all Adobe Experience Cloud solutions.

   **Important:**  Requests to some Adobe Experience Cloud solutions don't require the JavaScript library, but requests to Advertising Cloud require it.

   You should deploy the library on the web page from which your customers can submit access and delete requests, such as your company's privacy portal. The library helps you retrieve Adobe cookies (namespace ID: gsurferID) so that you can submit these identities as part of access and delete requests via the Adobe Experience Platform Privacy Service API.

   When the customer asks to delete personal data, the library also deletes the customer's cookie from the customer's browser.

   >[!NOTE]
   >
   >Deleting personal data is different than Opt-Out, which stops the targeting of an end user with audience segments. However, when a customer asks to delete personal data from Creative, DSP, or DCO, the library also sends a request to Advertising Cloud to opt out the customer from segment targeting. For advertisers with Search, we recommend that you provide your customers a link to [https://www.adobe.com/privacy/opt-out.html](https://www.adobe.com/privacy/opt-out.html), which explains how to opt out of audience segment targeting.

1. Identify your IMS Org ID and make sure it is linked to your Advertising Cloud accounts.

   An IMS Org ID is a 24-character alphanumeric string appended with @AdobeOrg. Most Adobe Experience Cloud customers have been assigned an IMS Org ID. If your marketing team or internal Adobe system administrator doesn't know your organization's IMS Org ID, or isn't sure if it's been provisioned, contact Adobe Customer Care at gdprsupport@adobe.com. You'll need the IMS Org ID to submit requests to the Privacy API.

   **Important:** Contact your company’s Advertising Cloud representative to confirm that all of your organization's Advertising Cloud accounts &mdash; including DSP accounts or advertisers, Search accounts, and Creative or DCO accounts &mdash; are linked to your IMS Org ID.

1. Use either the Adobe Experience Cloud Privacy Service API (for automated requests) or the Privacy Service UI (for ad-hoc requests) to submit access and delete requests to Advertising Cloud on behalf of your data subjects, and to check the status of existing requests.

   For advertisers who have a mobile app to interact with customers and launch campaigns with the DSP, you'll need to download the Privacy-ready Mobile SDKs for Experience Cloud. The Mobile SDKs allow businesses to set opt-out status flags, retrieve the data subject's device ID (namespace ID: deviceID), and submit requests to the Privacy Service API. Your mobile app will require an SDK Version 4.15.0 or greater.

   When you submit an access request, the Privacy Service API returns a data subject's information based on the specified cookie or device ID, which you then must return to the data subject.

   When you submit a delete request, the cookie ID or device ID and all cost, click, and revenue data associated with the cookie are deleted from the server.

   >[!NOTE]
   >
   >If your organization has more than one IMS Org ID, then you will need to submit separate GDPR API requests for each.

All of these steps are necessary for Advertising Cloud. For more information about these and other related tasks you need to perform using the Adobe Experience Platform Privacy Service, and where to find the items you'll need, see [www.adobe.io/apis/cloudplatform/gdpr.html](https://www.adobe.io/apis/experienceplatform/gdpr.html).

## Required Field Values in Advertising Cloud JSON Requests

"company context": 

* "namespace": **imsOrgID**
* "value": <*your IMS Org ID value*>

"users": 

* "key": <*usually the name of the data subject*> 

* "action": either **access** or **delete**

* "user IDs":

    * "namespace": **411** (which indicates the adcloud cookie space)

    * "value": <*the actual customer’s cookie ID value as retrieved from AdobePrivacy.js*>

* "include": **adCloud** (which is the Adobe product that applies to the request)

* "regulation": **ccpa** (which is the privacy regulation that applies to the request)

## Data Fields That Are Returned for Access Requests

The following is an example of an access response for Advertising Cloud.

'''
{
    "jobId":"12345AD43E",
    "action":"access",
    "product":"adCloud",
    "status":"complete",
    "results":{
        "userIDs":[
            {
                "namespace":"411",
                "userID":" Wqersioejr-wdg "
            }
        ],
        "receiptData":{
            "impressionCount":"100",
            "clickCount":5,
            "geo":[
                "United States of America",
                "San Francisco CA"
            ],
            "profile":[
                {
                    "pixelid":"111",
                    "ut1":"abc",
                    "ut2":"def",
                    "ut3":"ghi",
                    "ut4":"jkl",
                    "ut5":"mno"
                },
                {
                    "pixelid":"123",
                    "ut1":"abc",
                    "ut2":"def",
                    "ut3":"ghi",
                    "ut4":"jkl",
                    "ut5":"mno"
                }
            ],
            "matchingSegments":[
                {
                    "segmentName":"AP4 - Art/Culture - In-Market",
                    "segmentID":"kV1mPa2aqPNWKSNtf325",
                    "serviceProvider":"Adobe"
                },
                {
                    "segmentName":"EMEA - UK - Health Food Buyers",
                    "segmentID":"eP2oJ2UPsfsDVDhvlGewx",
                    "serviceProvider":"BlueKai"
                }
            ]
        }
    }
}
'''
