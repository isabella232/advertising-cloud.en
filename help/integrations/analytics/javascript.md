---
title: JavaScript Code for Analytics for Advertising Cloud
description: JavaScript Code for Analytics for Advertising Cloud
feature: integration with Adobe Analytics
exl-id: 184508ce-df8d-4fa0-b22b-ca0546a61d58
---
# JavaScript Code for Analytics for Advertising Cloud

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

*Advertisers with Advertising Cloud DSP only*

For Advertising Cloud DSP, the Analytics for Advertising Cloud integration tracks view-through and click-through site interactions. Click-through visits are tracked by the standard Adobe Analytics code on your webpages; the Analytics code captures the AMO ID and EF ID parameters in the landing page URL and tracks them in their respective reserved eVars. You can track view-through visits by deploying two lines of JavaScript code in your webpages.

On the first page view of a visit to the site, the Advertising Cloud JavaScript code checks to see if the visitor has previously seen or clicked on an ad. If the user has previously entered the site via a click-through or hasn't seen an ad, then the visitor is ignored. If the visitor has seen an ad and hasn't entered the site via a click-through during the [click lookback window](/help/integrations/analytics/prerequisites.md#lookback-a4adc) set within Advertising Cloud, then the Advertising Cloud JavaScript code uses the [Experience Cloud ID Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) to generate a supplemental ID (SDID), which is used to stitch data from Advertising Cloud to the visitor’s Adobe Analytics hit. Adobe Analytics then queries Advertising Cloud for the AMO ID and EF ID associated with the ad exposure. The AMO ID and EF IDs are then populated in their respective eVars. These values persist for a designated period (by default, 60 days).

Analytics sends site traffic metrics (such as page views, visits, and time spent) and any Analytics custom or standard events to Advertising Cloud hourly, using the EF ID as the key. These Analytics metrics then run through the Advertising Cloud attribution system to connect the conversions to the click and exposure history.

>[!NOTE]
>
>The Advertising Cloud JavaScript tracking logic occurs on the Adobe side and thus has virtually no impact to the page load time.
>
>In contrast, the logic for the DCM data connector to Analytics (using Google Campaign Manager 360) for Advertising Cloud DSP occurs on the client side. Client-side stitching slows down the page load and increases the risk of data loss. This occurs because the Analytics JavaScript must ping DoubleClick and wait for DoubleClick to pass back the last click/impression data to Analytics. When your DSP team sets up the DCM data connector, you must specify how long you're willing to delay the page.

## Deploying the JavaScript Code

The JavaScript library consists of two lines that allow Analytics and Advertising Cloud to communicate with each other. If the Analytics for Advertising Cloud integration was completed during the Advertising Cloud implementation, then you should have received this code with instructions on how to deploy it.

If you don't already have the code, then contact the Advertising Cloud support team.

### Where to Place the Code

The Analytics for Advertising Cloud JavaScript function must come after the Experience Cloud ID Service but before your Analytics App Measurement code so that the supplemental ID (SDID) can be included in your Analytics call.

![Code placement](/help/integrations/assets/a4adc-code-placement.png)

### Validating Code Deployment

You can perform validation using any packet sniffer type of tool (such as Charles, Fiddler, or Chrome Developer Tools) by comparing the values of the four IDs between the request going to Advertising Cloud and the request going to Analytics, as outlined below.

#### How to Confirm the Code with Chrome Developer Tools {#validate-js-chrome}

1. Open Chrome Developer Tools and click the **Network** tab.
1. Load a website page that contains the Analytics for Advertising Cloud JavaScript.
1. Filter the Network tab by “last” and review two rows:

     ![Filtering on last](/help/integrations/assets/a4adc-code-validation-filter-last.png)

     * The first row is the call to the JavaScript library and is titled last-event-tag-latest.min.js.
     * The second row is the call sending the request to Advertising Cloud. It begins as follows: `_les_imsOrgId=[your_imsOrgId_here]&_les_url=[your_encoded_url]`
     
         If you don't see the call to Advertising Cloud, then it might not be the first page view of your visit. For testing purposes, you can remove the cookie so that the next call will be the first page view for the corresponding visit:
         
          1. On the Application tab, find the “adcloud” cookie, and verify that the cookie contains “_les_v” (last visit) with a value of “y” and a UTC epoch timestamp that expires in 30 minutes.
          1. Delete the “ad cloud” cookie and refresh the page.
1. Filter on “/b/ss” to see the Analytics hit.

     ![Filtering on /b/ss](/help/integrations/assets/a4adc-code-validation-filter-bss.png)

1. Compare the ID values between the two hits. All of the values will be in query string parameters except for the report suite ID in the Analytics hit, which is the URL path immediately after /b/ss/.

     | ID | Analytics Parameter | Advertising Cloud Parameter |
     |--- |--- |--- |
     | Experience Cloud IMS Org | mcorgid | _les_imsOrgid |
     | Supplemental Data ID | sdid | _les_sdid |
     | Analytics Report Suite | The value after /b/ss/ | _les_rsid |
     | Experience Cloud Visitor ID | mid | _les_mid |

     If the ID values match, then the JavaScript implementation is confirmed. Advertising Cloud will send the Analytics server any click-through or view-through tracking details if they exist.

#### How to Confirm the Code with Adobe Experience Cloud Debugger

1. Open the [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/run-debugger.html) on your homepage.
1. Go to the **Network** tab.
1. In the **Solutions Filter** toolbar, click **Advertising Cloud** and **Analytics**.
1. In the **Request URL – Hostname** parameter row, locate “lasteventf-tm.everesttech.net.”
1. In the **Request – Parameters** row, audit the signals generated, similar to Step 3 in "[How to Confirm the Code with Chrome Developer Tools](#validate-js-chrome)."
     * Check to make sure the SDID parameter matches the Supplemental Data ID in the Adobe Analytics filter.
     * If the code isn't generating, then check to make sure the Advertising Cloud cookie has been removed in the Application tab. Once it's removed, refresh the page and repeat the process.

     ![Auditing Analytics for Advertising Cloud JavaScript code in Experience Cloud Debugger](/help/integrations/assets/a4adc-js-audit-debugger.png)

>[!MORELIKETHIS]
>
>* [Overview of Analytics for Advertising Cloud](overview.md)
>* [Prerequisites and Key Information for Implementing Analytics for Advertising Cloud](prerequisites.md)
