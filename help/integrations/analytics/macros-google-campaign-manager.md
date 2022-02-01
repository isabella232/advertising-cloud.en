---
title: Analytics for Advertising Cloud Macros for Google Campaign Manager 360 Ad Tags
description: Learn about Analytics for Advertising Cloud macros for Google Campaign Manager 360 ad tags
feature: Integration with Adobe Analytics
exl-id:
---
# Analytics for Advertising Cloud Macros for Google Campaign Manager 360 Ad Tags<!-- wording? correct terms? -->

*Advertisers with an Advertising Cloud-Adobe Analytics Integration Only*

*Applicable to Advertising Cloud DSP only*

If you use ad tags from Google Campaign Manager 360 for your Advertising Cloud DSP ads, you can append Analytics for Advertising Cloud parameters to your landing page URLs using the [`%p` macro](https://support.google.com/campaignmanager/table/6096962).

This allows Advertising Cloud to send click data for the ads to Adobe Analytics.<!-- Correct? -->

# Append the Macros to Your Google Campaign Manager 360 Ads

Within Google Campaign Manager 360, append to the following parameter to the landing page URL: `%pamo=!;`

You can specify the landing page URL in several ways. Instructions for each option are included in the following subsections.

The following is an example of the landing page URL formatted with the suffix.

```
https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;
```

>[!NOTES]
>
>
>* If the landing page URL includes a hash symbol (#), which is not common, then place the `amo` parameter before the hash symbol.
>* If no other parameters are included after the `amo` parameter, then add a parameter (for example, &a=b) after it. Example:`https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;&a=b#login`

## Configure the Advertiser-Level Landing Page URL Suffix

1. In the main menu, click the [!UICONTROL Advertisers] tab.
1. Click the advertiser name.
1. In the [!UICONTROL Landing page URL suffix] settings, include `%pamo!;` in the [!UICONTROL URL suffix] field.

## Configure the Campaign-Level Landing Page URL Suffix

1. In the main menu, click the [!UICONTROL Campaigns] tab.
1. Click the campaign name.
1. Click [!UICONTROL Properties].
1. In the [!UICONTROL Landing page URL suffix] settings, include `%pamo!;` in the [!UICONTROL URL suffix] field.	 

## Configure the Creative-Level Landing Page URL Suffix

1. In the main menu, click the [!UICONTROL Campaigns] tab.
1. Click the campaign name.
1. In the [!UICONTROL Views] menu, select [!UICONTROL Creatives].
1. Click the creative name.
1. In the [!UICONTROL Click tags] setting, include `%pamo!;` in the [!UICONTROL Landing page] column for the click tag.

# How Analytics for Advertising Cloud Macros Are Expanded in Advertising Cloud DSP

In Advertising Cloud DSP, when you create an ad that includes the Analytics for Advertising Cloud parameter (`amo`), the `ef_id` and `s_kwcid` macros are automatically appended to the click URL. The best practice is to check the tag in Advertising Cloud DSP to ensure that the `ef_id` and `s_kwcid` macros are present.

The following is an example of a Google Campaign Manager 360 [ins tag](https://support.google.com/campaignmanager/answer/6080468) as it appears in Advertising Cloud DSP.

```
<ins class='dcmads' style='display:inline-block;width:160px;height:600px'
data-dcm-placement='N6482.2155306TUBEMOGUL/B23486129.261313631'
data-dcm-rendering-mode='iframe'
data-dcm-https-only
data-dcm-resettable-device-id=''
data-dcm-app-id='' data-dcm-click-tracker='${TM_CLICK_URL}'
data-dcm-param-amo='ef_id=${TM_USER_ID}:${TM_DATETIME}:d&s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}'>
<script src='https://www.googletagservices.com/dcm/dcmads.js'></script>
</ins>
```

When a user clicks the ad<!-- ??? -->, Google Campaign Manager 360 sees `%pamo` in the URL suffix and dynamically inserts the value of the `amo` parameter into the URL.