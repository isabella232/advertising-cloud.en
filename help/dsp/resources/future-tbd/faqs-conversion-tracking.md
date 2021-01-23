---
title: FAQs About Advertising Cloud Conversion and Page View Tracking Tags
description: FAQs About Advertising Cloud Conversion and Page View Tracking Tags
---

# FAQs About Advertising Cloud Conversion and Page View Tracking Tags

The following apply to Advertising Cloud conversion tracking tags and page view tracking tags.

|  | JS Version 3 Tags | JS Version 2 Tags | Image Tags |
| --- | --- | --- | --- |
| Can be used on the same web page as another JS version | &mdash;  | &mdash; | n/a |
| Allows the use of multiple tags with the same advertiser user IDs on the same web page | YES | YES | &mdash; |
| Allows the use of multiple tags with different advertiser user IDs on the same web page | YES | &mdash; | &mdash; |
| Used by the Advertising Cloud tool in Adobe Dynamic Tag Manager and by Adobe Experience Platform Launch, and compatible with other tags generated using Dynamic Tag Manager and Experience Platform Launch | YES | &mdash; | &mdash; |
| Allows all conversions that originate from Apple Safari and Mozilla Firefox to be tracked when used with the Advertising Cloud JavaScript conversion mapping tag | YES | YES | NO |

>[!NOTE]
>
>* All new implementations use JavaScript Version 3.
>* Use JavaScript Version 2 tags only when the advertiser already has Version 2 tags on its web pages.
>* The best practice is to use JavaScript tags instead of image tags unless the site has a policy against using them.
>* JavaScript tags are required for advertisers who want to target audiences created in Adobe Experience Cloud, created in Adobe Audience Manager, or published to Adobe Experience Cloud from Audience Manager or Adobe Analytics.

>[!MORELIKETHIS]
>
>* [Generate an Advertising Cloud Conversion Tag](conversion-pixel-create.md)
