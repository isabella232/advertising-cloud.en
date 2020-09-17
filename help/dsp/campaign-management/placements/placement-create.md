# Create a Placement {#placement-create}

>[!Tip]
>
>Create placements based on specific campaign goals or reporting needs.

1. In the main menu, click **Campaigns Beta**.

1. Click the name of the campaign in which the placement will be included.

1. Above the data table, click **Create**. In the Placement Types section of the menu, click the placement type.

   The placement type determines the ad type that the placement can include.

1. Enter the [placement settings](placement-settings.md):

    1. Specify the Basics settings.

    1. In the Goals section, specify the Gross Budget and, optionally, specify additional placement goals.
       Some fields have default values that you can override.

       If the package to which the placement is assigned has package-level pacing, then your goals and pacing settings will reflect the package settings.

    1. (Optional) In the Geo-Targeting section, narrow down the locations that are included or excluded.
       If you don't specify specific locations, all locations are targeted.

    1. (Optional) In the Inventory Targeting section, narrow down the inventory sources to include or exclude.

       By default, all inventory sources are targeted.

    1. (Optional) In the Site Targeting section, narrow down the sites that you want to target, and specify any sites that you want to exclude.

    1. (Optional) In the Audience Targeting section:
    
      1. Narrow down the audience. This includes selecting audience segments to target within the placement.
      
      1. (For campaigns with people-level cross-device targeting; optional) When the placement targets one or more specific audiences, enable people-based cross-device targeting for the placement.
      
         People-based cross-device targeting is provided by LiveRamp using U.S. data only. The service is available to all advertisers at $0.35 CPM for impressions that are delivered by using the LiveRamp device graph (that is, for devices not found within the targeted audience segments).

    1. (Optional) In the Brand Safety and Media Targeting section, apply brand safety restrictions for your placements.

    1. (Optional) In the Tracking section, enter third-party event pixels or conversion pixels for ads in the placement.

1. Click **Create Placement**.

1. (Optional) Attach ads to the placement:

   1. Click **Attach an ad**.

   1.  Do either of the following:

      * To create a new ad:

         1. Click **Create a New Ad.**

         1. Specify the ad settings for [audio ads](/help/dsp/campaign-management/ads/ad-settings-audio.md), [connected TV](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md), [display ads](/help/dsp/campaign-management/ads/ad-settings-display.md),[mobile ads](/help/dsp/campaign-management/ads/ad-settings-mobile.md), [native ads](/help/dsp/campaign-management/ads/ad-settings-native.md), [pre-roll ads](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md), or new [survey ads](/help/dsp/campaign-management/ads/ad-settings-survey.md).
        
         1. Click "Save & Submit for Review."

         1. (Optional) For each additional ad you want to create for the placement, click **Attach Another Ad**, and then repeat Steps 1-3.

         1. If you won't attach any existing ads, click **I'm done for now**.

      * To attach existing ads in the campaign:
    
         1. Click **Select an Ad**.

         1. Next to the ad name, click **Select**.

         1. (Optional) For each additional ad you want to attach, click **Add Another Ad**, and then repeat the Steps 1-2.

         1. (Optional) To override the default flight period and ad rotation for specific ads in the placement:
         
            1. Click **Custom Schedule Ads**.

            1. Do any of the following:

               * To add a flight, click **Add Flight**, and then specify the start date and end date.
               
               * To add an existing flight to an ad, click **+** in the ad row for the flight column.

               * To remove an existing flight from an ad, click **x** in the ad row for the flight column.

               * (When multiple ads have the same flight) To rotate the ads unevenly, click **Even Rotation** in the flight information, and then enter the relative weight by which to rotate each ad, as a percentage.

                  The total weights must equal 100.

            1. In the upper right, click **Continue**.

            1. Review the flight details, and then click **Save & Finish**.

>[!MORELIKETHIS]
>
>* [About Placement Management](/help/dsp/campaign-management/placements/placement-about.md)
>* [Placement Settings](/help/dsp/campaign-management/placements/placement-settings.md)