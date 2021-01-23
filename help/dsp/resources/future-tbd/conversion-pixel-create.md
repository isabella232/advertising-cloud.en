---
title: Generate an Advertising Cloud Conversion Tag
description: Generate an Advertising Cloud Conversion Tag
---

# Generate an Advertising Cloud Conversion Tag

*Advertisers with Advertising Cloud Conversion Tracking Only*

<!-- Does DSP have clients who track conversions another way and submit conversion data via a feed rather than use our tracking? -->
<!-- For search, you have to specify transaction properties to track. Are there any caveats/differences for DSP clients? -->

1. Log into Advertising Cloud Search at https://enterprise-na.efrontier.com or https://enterprise-intl.efrontier.com.
1. In the main menu, click **Search > Tools > Conversion Tags**.
1. Specify the conversion tag settings.

     To track conversions on Safari browsers, you must use a JavaScript v2 or v3 tag.
     
     For more information about the differences between the tag types, see "[FAQs About Advertising Cloud Conversion and Page View Tracking Tags](ADD LINK)".
1. Generate the tag:
    * If the website uses HTTP, click **Generate Conversion Tag**.
1. If the website runs on a secure server (HTTPS), click **Generate Secure Conversion Tag**.
1. Copy the tag from the dialog box, and paste it into to the appropriate web pages as needed.

>[!NOTE]
>
> In Advertising Cloud Search, each property in the new conversion tag is automatically listed in Admin > Transaction Properties, even if it hasn't been implemented or the web pages it's on haven't received any clicks. This is different than the behavior of properties in tags created manually or elsewhere, which aren't listed in Admin > Transaction Properties until one of the web pages it's on has received a click. In all cases, however, each property is initially excluded from objectives, reports, and views until you explicitly make them available. Before you add the properties to objectives, consider first making the properties available and adding them to reports to verify when they receive clicks.

>[!MORELIKETHIS]
>
>* [FAQs About Advertising Cloud Conversion and Page View Tracking Tags](faqs-conversion-tracking.md)
