---
title: Advertising Cloud DSP Macros
description: Reference the available macros for general tracking and to track clicks on third-party display ads.
feature: Ads
exl-id: e31cc2e5-ad1f-4555-a87b-0e4c3731fe5f
---
# Advertising Cloud DSP Macros

A macro is a short command or shorthand for an instruction and usually follows the format `${MACRO_NAME}`. The Advertising Cloud DSP ad server executes macros when the ad is served or clicked.

Macros are most commonly used during trafficking of third-party and custom creative code or metadata (such as third-party pixels).

## General Tracking Macros

Use general tracking macros across all ad and tag types to pass back specific data, as required.

| Macro | Description |
| --------------- | ---------------------- |
| `${USER_ID}` | User identifier for all device types. |
| `${TM_RANDOM}` | Cachebuster: a random number between 1 and 1000000 |
| `${TM_PLACEMENT_ID_NUM}` | The placement ID |
| `${TM_SITE_URL_URLENC}` | The URL passed in the bid request; URL-encoded |
| `${TM_SITE_DOMAIN_URLENC}` | The page subdomain parsed from the URL in the bid request; URL-encoded |

## Click Macros for Third-Party Display Ads

To accurately track clicks for ads using third-party display tags, DSP requires a display click macro. Only one version of the macro is required; the relevant macro depends on the type of tag.

| Macro | Description |
| --------------- | ---------------------- |
| `${TM_CLICK_URL}` | Redirect URL that enables ad servers to track and count ad clicks in the platform |
| `${TM_CLICK_URL_URLENC}` | Redirect URL that enables ad servers that require URL encoding to track and count ad clicks in the platform |

DSP automatically inserts display click macros in a display tag when you:

* Export ad tags from an Advertising Cloud ad server partner <!-- [Needs PM confirmation.] -->
* Bulk upload Flashtalking or Google DoubleClick for Advertisers ad tags directly in DSP

If a click macro is missing when you build a display ad, DSP displays a warning message, which prompts you to manually insert the appropriate display click macro in the correct area of the tag.

>[!MORELIKETHIS]
>
>* [Audio Ad Settings](/help/dsp/campaign-management/ads/ad-settings-audio.md)
>* [Audio Ad Settings](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md)
>* [Audio Ad Settings](/help/dsp/campaign-management/ads/ad-settings-display.md)
>* [Audio Ad Settings](/help/dsp/campaign-management/ads/ad-settings-mobile.md)
>* [Audio Ad Settings](/help/dsp/campaign-management/ads/ad-settings-native.md)
>* [Audio Ad Settings](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md)
