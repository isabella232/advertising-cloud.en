---
title: Create Multiple Third-party Ads
description: Create Multiple Third-party Ads
---
# Create Multiple Third-party Ads

You can create up to 500 third-party ads at a time by uploading tags that point to creative assets hosted on third-party ad servers. You can include tracking pixels for the ads.<!-- The bulksheet template for other ad servers says you can include 200. Which is it: 200 or 500? -->

You can upload either DoubleClick and Flashtalking tag sheets or  a manually-populated file using the provided template.

To create a single third-party ad, see [Create an Ad](ad-create.md).

>[!TIP]
>
> The best practice is to use third-party ads that are served securely using HTTPS. URLs served using HTTPS begin with "https."

1. In the main menu, select **Campaigns Beta**.

1. Click the name of the campaign in which the ad will be included.

1. Above the data table, click **Create**. In the Ad Types section of the menu, click **Bulk upload ads**.

1. Select the ad server on which the ad is hosted: *DoubleClick*, *Flashtalking*, or *Other*.

1. (DoubleClick and Flashtalking ads) Select the tag type to use for each video asset and each display asset. The available options vary by ad server.

1. (Ads on all ad servers except DoubleClick and Flashtalking) Click **Download this template** to download a template in Microsoft Excel spreadsheet (XLSX) format, which you can populate with ad data and save locally. The required columns include Ad Name, VAST/VPAID URL or Ad Tag, and Ad Types.

1. Click **Upload** and select a file in .xlsx or .xls formats from your device or network.

   For DoubleClick and Flashtalking ads, upload unedited tag sheets from the ad server. For other ad servers, use the template you downloaded in Step 3.

1. After the upload is complete, click **Start Building Ads**.

1. Review the details and status of each ad:

   1. Review the status of each ad, which is based on validation checks on the uploaded tag.
   1. (Optional) Do any of the following for each ad:
      * To preview an ad, click ![play](/help/dsp/assets/play.png) in the ad row.
      * To edit the ad details, click ![edit](/help/dsp/assets/edit.png), edit the details, and then click **Save**.
      * To remove an ad, click **X** in the ad row.

1. Click **Create *N* Ad(s)**.

1. Do one of the following:

   * Click **Done**.

   * (If an ad is rejected; optional) To edit the ad record and resubmit the ad for review:
      1. Click the ad name.
      1. Edit the ad settings.
      1. Click **Save & submit for review**.

>[!MORELIKETHIS]
>
>* [About Ad Management](ad-about.md)
>* [Create an Ad](ad-create.md)
>* [Available Ad Types](ad-types.md)
>* [Ad Specifications](https://education.tubemogul.com/wp-content/uploads/2020/08/Adobe_Avstg_Cloud-Ad-Specs-20201.pdf)
