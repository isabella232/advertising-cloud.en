---
title: Tracking Pixels
description: Tracking Pixels
---

# Tracking Pixels

You can optionally add third-party tracking pixels to your ads to track a variety of integration events, including impressions, clicks, and completions.

You can add third-party tracking pixels to the following ad settings.

## Basic Tab

* Click URL: Add clickthrough redirect pixel here (should be click pixels not jump tags)

## Companion Tab

Add any companion banner 3rd party clickthrough pixels in this section. If you want to also track companion impression, you will need to create an iframe.

## Pixel Tab


* Integration Events shown in the drop down will change by type of ad unit you've selected:

    * For In-Stream units, fire the pixel on the impression or quartile completion.
    * For In-Display units, fire the pixel on the impression, view, quartile completions and clicks.
    * Our BrandSights surveys can fire the following 3rd party pixels:

        * Survey Start: The first question has been answered. (Only fired if there is more than one question.)
        * Survey Complete: The last (or only) question has been answered.

* Pixel URL: drop the 1x1 3rd party pixel here
* Pixel Name: name the pixel. Recommended to be specific to avoid confusion
* Pixel Provider: Selecting the right provider is important as one of our inventory providers- Google AdX uses this as an identifier and without the proper selection may reject the ad and affect your delivery.

    * Select Nielsen if you are adding a Nielsen pixel.
    * Select ComScore if you are adding a ComScore pixel.
    * Select None for all other 3rd party ad servers.

* Once you are finished, Save & Close. Repeat the steps if you have multiple pixels to attach.


>[!TIP]
>
> Use a a web debugging tool like Charles or Fiddler to verify pixel fires before launching the campaign. 

## Best Practices

* Always double check if your 3rd party pixels are a click redirect or 1x1 image pixel. To verify, drop the pixel on a browser. If it redirects, it's a click tracker; if it shows an empty blank browser, it's a 1x1 image pixel that can track any integration event.
* Download a web-debugging tool like [Fiddler](https://www.telerik.com/fiddler) or  [Charles](https://www.charlesproxy.com/) to help pixel check and verify that proper pixels are firing.

* Compare a third-party tracking report with Advertising Cloud DSP within 1 or 2 days of campaign launch and check for discrepancies. If there are discrepancies >10%:

    * Follow the below instructions to doublecheck pixel implementation:

        * Run web-debugging tool (Fiddler or Charles)
        * In Advertising Cloud DSP, go to –> Ads–> Options–> Edit
        * While the ad is playing on the preview page, the web-debugging tool will record all pixels that are firing.
        * Verify the pixels fired with your 3rd party pixel map.

* If you're using a SWF file, then you'll need to include the tracking pixels within the file
* Verify your campaign pixel set-up with our Pixel Q&A tool located in the Tools section on the top navigation bar.
