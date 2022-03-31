---
title: About Ad Management in Advertising Cloud DSP
description: Learn about ad management.
feature: DSP Ads
exl-id: 72c8bbef-d09c-4cf4-994d-99578d043d39
---
# About Ad Management in Advertising Cloud DSP

<!-- add "The Ads View (Dashboard?)" section -->

Advertising Cloud DSP supports ad delivery via manual creation of native display ads or direct upload of third-party ad serving tags (such as Google, Flashtalking, or Sizmek). You can upload third-party tags individually or in bulk. Bulk uploads use partner tag sheets or a bulk tag template. 

<!-- The bulk upload feature requires you to either a) upload DoubleClick and Flashtalking tag sheets or b) download a template, input your tags into the template, and then re-upload the template. -->
<!-- need a list of all supported third-party ad servers; see file in future-tbd folder -->

Once your ads are set up, you'll need to attach each ad to a placement, which includes the targeting parameters (such as geo, audience, device, and inventory targeting) that will control how your campaign will deliver. You can attach a single ad to one or multiple placements.

## Available Ad Types

* Audio
* Connected TV
* Display
* Mobile
* Native Display
* Pre-Roll

For more information about these ad types, see [Available Ad Types](ad-types.md) and the complete [Ad Specifications](/help/dsp/assets/ad-specs.pdf).

## Advertising Cloud DSP Ad Approvals

When you create an ad, Advertising Cloud DSP reviews it for sensitive categories, click URL functionality, and preview rendering.

Initially, you'll see a red dot in the [!UICONTROL Status] column. The review process normally takes 24-48 hours. A broken ad, however, may have a pending status for longer than 48 hours so you have time to fix errors before the ad is rejected. Rejected ads include a reason for the rejection.

When DSP approves an ad, you'll see a green dot in the Status column.

![approval indicator in [!UICONTROL Status] column](/help/dsp/assets/ad-approval-status.png)

>[!NOTE]
>
>Your ad will only be served if both DSP and the SSP have approved the creative. Each SSP has its own approval requirements and process.

>[!MORELIKETHIS]
>
>* [Create a Single Ad](ad-create.md)
>* [Create Multiple Third-party Ads](ad-create-multiple.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](/help/dsp/assets/ad-specs.pdf)
