# Create a Survey  {#survey-create}
### Platform Setup
1.	**Creating Suppression Pixels:** 
>
When running Surveys, it is important not to serve the same question to the same person twice to avoid biasing the results. The way we do this is by creating a pixel that fires when somebody starts the Survey to ensure that anybody who receives the Survey will not be served it again. To create the suppression pixel, follow instructions below:
1. >
    1. Go Tools and Segments.
    1. Click New Custom Segment.
    1. Name the segment something like 'Survey Start'.
    1. You will then need to attach this pixel when you come to creating the survey ad.
    1. To find the pixel, click the gear icon next to the segment you just created and click get pixel. Make sure you use the pixel that collects users exposed to an ad.
> 
**Creating the Survey** *Navigate to the Campaigns section of the platform. Then go to Surveys on the left-hand panel.*
>    
Select your Survey type:
>
  1. In Display (300x250)
    * Collection Methodology: Desktop Cookies
      * Format:
        * Display 
          * Video (NOTE: PR Surveys are VPAID JS)
  1. Pre-Roll (400x300)
     * Format: 
        * Pre-Roll
          * CTV & PTV: Utilizes IP Addresses to target users via Desktop Cookies
  1. Mobile (Interstitial)
  1. Mobile Web: 
     * Collection Methodology: Mobile Cookies
     * Utilizes IP Addresses to target users via Mobile Cookies
  1. Mobile App: 
      * Collection Methodology: Device IDs
         * CTV: Utilizes IP Addresses to target users via Device IDs
>
You will now need to fill out the Survey details.
1. Make sure the Advertiser is correct and provide your survey with a name.
  1. If you have more than one question, then you will need to click Add a Question and repeat the next stages.
1. Select either Single Answer or Multiple Answers.
1. Choose your Category depending on what you are looking to measure.
1. Type your question in the Question Text field.
  1. Decide whether you would like to Randomize your answers. Doing this can avoid biasing results.
1. Start typing in the answers to your question below.
  1. If your last answer is 'none of the above' and you have Randomize Answers selected, make sure you select Lock in Place next to this answer.
  1. If you have a multiple answer response such as 'all of the above' then you will need to click the drop-down button and either choose Selects All or De-selects All.
>


**Creating the Ad**
1. Once you have finished creating the survey, you will be taken directly through to the Ad Editor. The survey you have just created will automatically be linked to the ad, so we advise clicking Start Ad and checking the survey previews as it is intended to.
   1. Under the Basic tab you will be able to name your survey which is important if you have multiple surveys in the same campaign.
   1. If the product/service, you are advertising is 18+ then you have the option to ask a predetermining question by clicking Enable Age Gate. This will prevent you from delivering the survey to under 18-years of age. 
   1. You now need to append the suppression pixel that you created earlier to the ad. To do this, navigate to the Pixel tab and click Create Pixel. Select the integration event to survey start and the Pixel Type as IMG URL. Paste in the pixel and name it 'Survey Start'. Leave the pixel provider as none. Click Save & Submit for Review and that's the survey creation process completed.  *This is based on the user answering truthfully.*

   1. Edit the [survey ad settings](ad-settings-survey.md).
   1. (Optional) Click "Save & Submit for Review."
   
      The ad is automatically created, even if you don't save and submit any changes for review.


Creating the Placements
1. Now that you have created your survey, you will need to create control and exposed placements per survey. One of these placements will be targeting your exposed audience (people who have seen your ad) and the other will be your control placement (people who haven't seen your ad). This guide will not detail the entire placement setup process as the same rules apply to the media placements which should already have been created.
    1. If you are testing two creatives, you would have 1 control and 2 exposed (exposed to creative a. and creative b.  or if you were testing 2 audiences you would have 4 placements, 2 control mirroring your media placements and 2 exposed (audience a and audience b) 
    1.	You will need to create Survey Complete, Survey Start, and Exposed Media pixels. 
1.	Navigate to the Campaigns section and click New Placement. Then click Surveys and match your Survey placement type with the Survey type you created earlier.
1. Insert and select all the required placement settings.
  1. This placement will be the control placement so under survey settings, make sure Control is set to 'Yes'. 
1. Navigate to audience segments under audience targeting and click the Custom tab.
  1. Select Include next to the exposed media audience segment and the survey start segment.
  1.	Before clicking Add, make sure that the targeting setting is set to NOT so that you are negatively targeting these audience.
  1. If your other required placement settings are complete you can now, click Create Placement.
1. You will now need to repeat this process for the exposed audience.
  1. For the exposed placement you will need to change Set as Control to 'No'.
1. Under audience segments you will need to Add the media exposed segment as OR'd together and the survey start as NOT. To create two separate audience targeting rules, you will need to click the '+' and then add your second targeting type. Once you have saved your placement you are now ready to set the surveys live.
> **NOTES:** 
  1. ALL Control and Exposed placements should be anti-targeting survey starts
  1. ALL Control placements should be anti-targeting exposed groups
  1. ALL Control placements MUST mirror the targeting on the media placements (you need to use the same 3rd party, 1 party, topic targeting, contextual targeting, etc. as your media placement on your control placement).
  1. For exposed placements, you need to ensure exposed placements are anti- targeting other exposed groups if there are multiple. 
  1. For example, Audience A is being targeted, you need to suppress Audience B and survey starts to make sure your exposed groups stay clean 


>[!MORELIKETHIS]
>
>* [About Survey Management in Advertising Cloud DSP](survey-about.md)
>* [Survey Settings](survey-settings.md)
>* [Create an Additional Ad from a Survey](survey-create-additional-ad.md)
>* [Survey Ad Settings](/help/dsp/campaign-management/ads/ad-settings-survey.md)
>* [Best Practices for Survey Optimization](survey-best-practices-optimization)
>* [View Survey Performance](survey-view-performance.md)
