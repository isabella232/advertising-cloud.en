# About Audience Management in Advertising Cloud DSP {#audience-about}

In Advertising Cloud, you can create and manage audience segments and audience sets, which you can use as targets for your placements:

* You can collect your own first-party audience data by creating and implementing segments. You can later retarget users in the segment with ads or prevent users in the segment from receiving ads. You can create the following types of segments:

   * [Custom segments](/help/dsp/audiences/audience-create-custom-segment.md) to track a) users exposed to ads from desktop, mobile, and CTV devices and b) users who visit specific webpages.

   * [CCPA opt-out-of-sale segments](help/dsp/audiences/audience-create-ccpa-opt-out-segment.md) to track the users IDs from consumer opt-out-of-sale requests on your website, per the California Consumer Privacy Act (CCPA). You can retrieve monthly reports of the user IDs from opt-out-of-sale requests.
   
      For more information about Advertising Cloud support for CCPA opt-out-of-sale requests, see [Adobe Advertising Cloud Support for the California Consumer Privacy Act: Consumer Opt-out Support](https://docs.adobe.com/content/help/en/advertising-cloud/all/privacy/ad-cloud-ccpa-opt-out-of-sale.html).

* You can create an audience library of [reusable audiences](/help/dsp/audiences/audience-create-reusable-audience.md). Saved audiences are composed of any of your available audience segments and any of your other saved audiences. Any changes you make to a saved audience are automatically applied to all placements that target or exclude the audience and to all other audiences that include the saved audience.

   Saved audiences allow media planners to group audiences as needed, by including and excluding multiple segments using complex Boolean logic. The size of each individual segment and the total audience size are indicated as you build an audience. Campaign executioners can then simply select one or more saved audiences as placement targets rather than manually configure audience targets for each placement.

Additional audience types are also available for placement targeting.

## Importing First-party and Third-party Data Segments

Advertising Cloud can import your own first-party data segments from your data management platform (DMP) and provide them to any set of advertisers, as needed.

Advertising Cloud can also import custom third-party segments, including complex combinations of third-party segments. You can provide the segments to any set of advertisers, as needed.

Contact your Account Manager for more information.

## Audiences Available as Placement Targets

You can target your placements to all of the following types of audiences.

* All user-created audience sets that were saved in Advertising Cloud DSP/TV.

* All user-created audience segments that were created in Advertising Cloud DSP/TV:

   * Custom segments for users who visited specific webpages and users exposed to impressions of specific ads.
   
   * CCPA opt-out-of-sale audience segments for users who submitted opt-out-of-sale requests on your website, per the California Consumer Privacy Act (CCPA).

* All of your imported first-party data segments.

* All of your imported custom third-party data segments.

* (Placements targeting the U.S. only) [All third-party data segments available to Advertising Cloud DSP customers from over 30 providers](/help/dsp/audiences/audience-third-party-data-providers.md), including Acxiom, Datalogix, eXelate (Nielsen), Lotame, Oracle, Quantcast, and many more.

   You can target specific segments, which target users based on audience data (for example, users with specific demographics, interests or intents, and/or behavioral profiles). You can browse by data provider and category, search for segments by name or segment ID, or filter the results by data provider, total segment size, web browser count, or devices count.
   
   Third-party segments incur additional fees, which are indicated next to each segment name.

* (Advertisers with Adobe Experience Cloud, Adobe Audience Manager, or Adobe Analytics who use Advertising Cloud JavaScript conversion tags only) All of your available first-, second-, or third-party audience segments created in Adobe Experience Cloud, created in Audience Manager, or published to Adobe Experience Cloud from Audience Manager or Analytics.

   Pricing for the use of the segments is pre-negotiated and isn't visible in Advertising Cloud.  <!-- Verify -->
   
   Segments from Adobe Experience Cloud are available about an hour after you create or publish them in Adobe Experience Cloud. Segments coming directly from Audience Manager are available about 24 hours after you create them. <!-- Verify all -->
   
   >[!NOTE]
   >
   >See the documentation for [Audience Manager](https://docs.adobe.com/content/help/en/audience-manager/user-guide/aam-home.html), [Analytics](https://docs.adobe.com/content/help/en/analytics/landing/home.html), and [Adobe Experience Cloud](https://docs.adobe.com/content/help/en/core-services/interface/audiences/audience-library.html) for information about setting up and collecting data for segments in those solutions.

## Audience Size Data

Within saved audience settings and placement settings, you can see detailed audience size data:

* The total and active deduplicated audience size across all selected segments and saved audiences is displayed, and you can view details by device type (browser, mobile, or connected TV).

   ![the combined audience size](/help/dsp/assets/audience-size.png)
   
* For individual segments and saved audiences, the total audience size and CPM (when applicable) are displayed next to the segment name. You can view more details about the segment, including the size by device type (browser, mobile, or connected TV). For saved audiences, the total size is the deduplicated total.

   ![the individual segment size](/help/dsp/assets/audience-size-segment.png)

## The Audiences Views

### The All Audiences View

In the All Audiences View, or Audience Library, you can save and manage reusable audiences, which include groups of audience segments and even other saved audiences. You can use audiences as targets for multiple placements. The number of placements in which each audience is used is indicated next to the placement name.

You can edit, clone, delete, export, or share any audience.

### The Segments View

In the Segments view, all users can create additional custom segments.

The Segments view also lists the following segment types:

* All user-created custom segments available to the user.

   You can view tracking tags for any of the custom segments you created, and share those segments with other users. You can also edit or delete the custom segments you created.

   You can't edit or share custom segments that other users have shared with you.

* All imported first-party segments available to the user.

   You can't edit or share first-party segments that were shared with you. Contact your Account Manager if you need to share first-party segments with additional users.

* All custom third-party segments available to the user.

   You can't edit or share third-party segments that were shared with you. Contact your Account Manager if you need to share third-party segments with additional users.

>[!MORELIKETHIS]
>
>* [Create a Reusable Audience](audience-create-reusable-audience.md)
>* [Audience Settings](audience-settings.md)
>* [Syntax for Audience Segment Logic](audience-segment-logic-syntax.md)
>* [Create and Implement a Custom Segment](audience-create-custom-segment.md)
>* [Create and Implement a CCPA Opt-Out-of-Sale Segment](audience-create-ccpa-opt-out-segment.md)
>* [Available Third-party Data Providers](audience-third-party-data-providers.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)
