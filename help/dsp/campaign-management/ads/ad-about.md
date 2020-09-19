# About Ad Management in Advertising Cloud DSP {#ad-about}

Advertising Cloud DSP offers two ways to serve your ads:

* Advertising Cloud DSP will serve your ads for free when you upload your own assets (such as display banners, video assets, audio files, or URLs) directly to DSP. For DSP-served assets, you have access to additional features, such as overlays.

* If you use a third-party ad server (such as Google, Flashtalking, or Sizmek), you can upload your third-party ad serving tags to DSP individually or in bulk. The bulk upload feature requires you to either a) upload DoubleClick and Flashtalking tag sheets or b) download a template, input your tags into the template, and then re-upload the template.<!-- need a list of all supported third-party ad servers; see file in future-tbd folder -->

Once your ads are set up, you'll need to attach each ad to a placement, which includes the targeting parameters (such as geo, audience, device, and inventory targeting) that will control how your campaign will deliver. You can attach a single ad to one or multiple placements.

## Available Ad Types

* Audio
* Connected TV
* Display
* Mobile
* Native
* Pre-Roll
* Survey

For more information about these ad types, see [Available Ad Types](ad-types.md) and the complete [Ad Specifications](https://education.tubemogul.com/wp-content/uploads/2020/08/Adobe_Avstg_Cloud-Ad-Specs-20201.pdf).

## Special Ad Features

The following features are available for DSP-served ads only.

### Companion Banners

Companion banners are served alongside [pre-roll ads](ad-settings-pre-roll.md) or (with some publishers) [audio ads](ad-settings-audio.md) and can help reinforce brand and message association.

>[!NOTE]
>
>* Not all publishers allow companion banners. The publishers who do allow companion banners don't guarantee companion banner impressions.
>* Companion banners from third-party ad tags may not always available for preview.

You can upload your own companion banner asset or upload a third-party iFrame or script banner tag from a certified third-party ad serving partner.

### Overlays

Overlays help with persistent branding throughout the video and can drive additional clicks. The overlay feature is available for [interactive pre-roll ads](ad-settings-pre-roll.md) and for [mobile ads in interactive and tap-to-play formats](ad-settings-mobile.md).

See the [Best Practices for Designing Overlays](/help/dsp/campaign-management/ads/ad-best-practices-overlays.md)

### Teasers

A teaser is an eye-catching image that entices the viewer to play an ad. Teasers apply only to mobile tap-to-play ad formats.

## Advertising Cloud DSP Ad Approvals

When you create an ad, Advertising Cloud DSP reviews it for sensitive categories, click URL functionality, and preview rendering.

Initially, you'll see a red dot in the Status column. The review process normally takes 24-48 hours. A broken ad, however, may have a pending status for longer than 48 hours so you have time to fix errors before the ad is rejected. Rejected ads include a reason for the rejection.

When DSP approves an ad, you'll see a green dot in the Status column.

![approval indicator in Status column](/help/dsp/assets/ad-approval-status.png)

>[!NOTE]
>
>Your ad will only be served if both DSP and the SSP have approved the creative. Each SSP has its own approval requirements and process.

>[!MORELIKETHIS]
>
>* [Create an Ad](ad-create.md)
>* [Create Multiple Third-party Ads](ad-create-third-party.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](https://education.tubemogul.com/wp-content/uploads/2020/08/Adobe_Avstg_Cloud-Ad-Specs-20201.pdf)
